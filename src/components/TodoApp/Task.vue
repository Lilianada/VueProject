<template>
    <section :key="task.id" v-for="task in tasks">
        <p class="task-name"> {{ task.name }}</p>
    </section>
</template>

<script>
    export default {
        name: "Task",
        props: {
            task: Array,
        },
        
    }
</script>