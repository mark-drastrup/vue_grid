<template>
  <header>
    <input type="text" v-model="textValue" />
    <span>Profile</span>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
  data() {
    return {
      textValue: ""
    };
  }
};
</script>

<style lang="scss">
header {
  border-bottom: 1px solid black;
  display: grid;
  grid-template-rows: auto;
  grid-template-columns: 1fr 1fr;
  justify-content: space-between;
  align-content: center;
}

input {
  justify-self: start;
}

span {
  justify-self: end;
}
</style>