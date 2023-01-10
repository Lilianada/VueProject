<template>
  <div id="counter">
    <button @click="increment">Increment</button>
    <span> {{ count }} </span>
    <button @click="decrement">Decrement</button>
  </div>
</template>

<script>
export default {
  name: "counter",
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count++;
      console.log("incremented")
    },
    decrement() {
      this.count--;
    },
  },
};
</script>
