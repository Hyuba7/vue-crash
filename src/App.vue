<template>
  <div id="app">
    <Todos v-bind:todos="todos" />

    <!-- <datas /> -->
  </div>
</template>

<script>

import Todos from "./components/Todos";

export default {
  name: "App",
  components: {
    Todos,
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          title: "Todo 1",
          completed: false,
        },

        {
          id: 2,
          title: "Todo 2",
          completed: true,
        },

        {
          id: 3,
          title: "Todo 3",
          completed: true,
        },
      ],
    };
  },
};
</script>

<style>
</style>
