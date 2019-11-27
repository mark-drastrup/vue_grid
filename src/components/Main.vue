<template>
  <section>
    <header-section />
    <list />
  </section>
</template>

<script>
import HeaderSection from "./Header.vue";
import List from "./List.vue";
export default {
  name: "MainSection",
  components: { HeaderSection, List }
};
</script>

<style lang="scss" scoped>
section {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 6% 1fr;
}
</style> 