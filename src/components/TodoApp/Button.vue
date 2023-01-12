<template>
  <button class="add-button" :style="{background: color}" @click="onClick()" >{{ text }}</button>
</template>

<script>
export default {
  name: "add-button",
    props: {
        text: String,
        color: String,
    },
    methods: {
        onClick(){
            console.log("clicked")
        }
    }
};
</script>
