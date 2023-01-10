<template>
  <div id="test">
    <h1>Welcome {{ name }} to Vue Family</h1>
  </div>
</template>

<script>
export default {
  name: "test",
  data() {
    return {
      name: "Lilian Ada",
    };
  },
};
</script>

// import { createApp } from 'vue' // test.mount('#test')
