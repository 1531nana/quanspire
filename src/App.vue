<template>
  <Header />
  <Dropdown />
  <Actions />
  <Table />
</template>

<script>
import Header  from "./components/Header.vue";
import Dropdown  from "./components/Dropdown.vue";
import Actions  from "./components/Actions.vue";
import Table  from "./components/Table.vue";

export default {
  name: 'App',
  components: {
    Header,
    Dropdown,
    Actions,
    Table
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff8c;
  /* color: #2c3e50; */
}
</style>
