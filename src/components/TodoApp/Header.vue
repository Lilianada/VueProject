<template>
  <header class="head-section">
    <h3 class="todo-head">Todo App</h3>
    <Button text="Add Task" color="green" />
  </header>
</template>

<script>
import Button from "./Button.vue";

export default {
  name: "header",
  components: {
    Button,
  },
};
</script>
