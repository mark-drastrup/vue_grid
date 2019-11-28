<template>
  <section :class="showInfoBox === false ? 'grid1' : 'grid2'">
    <info-table />
    <info-box v-if="showInfoBox" />
    <button @click="show">Show Info</button>
  </section>
</template>

<script>
import InfoTable from "./InfoTable.vue";
import InfoBox from "./InfoBox.vue";
export default {
  name: "List",
  components: { InfoTable, InfoBox },
  data() {
    return {
      showInfoBox: true
    };
  },
  methods: {
    show() {
      this.showInfoBox = !this.showInfoBox;
    }
  }
};
</script>

<style lang="scss" scoped>
section {
  display: grid;
  grid-template-rows: 1fr;
}

.grid1 {
  grid-template-columns: 1fr;
}

.grid2 {
  grid-template-columns: 4fr 1fr;
}
</style>