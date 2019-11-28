<template>
  <section class="sidebar">
    <ul>
      <li>Menu Item 1</li>
      <li>Menu Item 2</li>
      <li>Menu Item 3</li>
      <li>Menu Item 4</li>
    </ul>
    <p>Settings</p>
  </section>
</template>

<script>
export default {
  name: "Sidebar"
};
</script>

<style lang="scss" scoped>
.sidebar {
  border-right: 1px solid black;
  align-content: space-between;
  display: grid;
}
</style>