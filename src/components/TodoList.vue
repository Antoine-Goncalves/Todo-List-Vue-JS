<template>
  <TodoInputText />
</template>

<script>
import TodoInputText from "@/components/TodoInputText.vue";
export default {
  components: {
    TodoInputText
  },
  data() {
    return {
      todos: []
    };
  }
};
</script>

<style>
</style>