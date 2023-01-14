<template>
  <section class="todo-section">
    <Header />
    <Task :task="tasks" />
  </section>
</template>

<script>
import Header from "./Header.vue";
import Task from "./Task.vue";
export default {
  name: "todo",
  components: {
    Header,
    Task
  },
  data () {
    return {
        tasks: Array
    }
  }
};
</script>
