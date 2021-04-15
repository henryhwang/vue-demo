<template>
    <div>
        <Task v-for="task in tasks" :key='task.id' :title="task.title"></Task>
    </div>
</template>

<script>
import Task from './Task'
export default {
    name: "Tasks",
    components: {
        Task
    },
    props: ['tasks']
}
</script>

