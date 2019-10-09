<template>
  <div id="app" class="container">
    <h1 class="title is-1 has-text-success">My Todo List</h1>
    <TodoList />
  </div>
</template>

<script>
import TodoList from "@/components/TodoList.vue";

export default {
  name: "app",
  components: {
    TodoList
  }
};
</script>

<style lang="scss">
.container {
  margin: 10rem 5rem 0 10rem;
}
</style>
