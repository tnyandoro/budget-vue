<template>
    <div :key="task.id" v-for="task in tasks">
        <Task :task="task" />
    </div>
</template>

<script>
import Task from './Task.vue'

export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Tasks',
    props: {
        tasks: Array
    },
    components: {
        Task
    }
}
</script>
<style>

</style>