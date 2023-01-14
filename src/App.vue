<template>
  <div id="app">
    <Todo />
  </div>
</template>

<script>
import Todo from "./components/TodoApp/Todo.vue";

export default {
  name: "app",
  components: {
    Todo,
  },
  data() {
    return {
      tasks: []
    };
  },
  created() {
    this.tasks = [
      {
        id: 1,
        name: "Do my laundry",
        time: "10:00am",
        status: "pending",
      },
      {
        id: 2,
        name: "Do my Alt-school assignment",
        time: "11:00pm",
        status: "done",
      },
      {
        id: 3,
        name: "Learn Vue js",
        time: "12:00pm",
        status: "pending",
      },
    ];
  },
};
</script>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
