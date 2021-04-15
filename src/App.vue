<template>
  <Tasks :tasks="this.tasks" />
</template>

<script>
import Tasks from './components/Tasks.vue'

export default {
  name: 'App',
  components: {
    Tasks
  },
  data() {
    return {
      tasks: []
    }
  },
  created: function() {
    this.tasks = [{
      id: 1,
      title: "Task 1"
    }, {
      id: 2,
      title: "Task 2"
    }, {
      id: 3,
      title: "Task 3"
    }]
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
