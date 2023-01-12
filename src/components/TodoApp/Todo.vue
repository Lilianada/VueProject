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
  created() {
    this.tasks = [
        {
            id: 1,
            name: "Do my laundry",
            time: "10:00am",
            status: "pending"
        },
        {
            id: 2,
            name: "Do my Alt-school assignment",
            time: "11:00pm",
            status: "done"
        },
        {
            id: 3,
            name: "Learn Vue js",
            time: "12:00pm",
            status: "pending"
        }
    ]
  }
};
</script>
