<template>
  <div class="todo-item" v-bind:class="{'is-complete':todo.completed}">
    <p>
      <input type="checkbox" v-on:change="markComplete">
      {{todo.title}}</p>
  </div>
</template>

<script>
export default {
  name: "TodoItem",
  props: ["todo"],
};
</script>

<style scoped>
.todo-item {
  background: #f4f4f4;
  padding: 10px;
  border-bottom: 1px;
}

.is-complete {
  text-decoration: line-through;
}
</style>