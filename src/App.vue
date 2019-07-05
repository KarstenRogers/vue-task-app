<template>
  <div id="app" class="container">
    <h1>Task List</h1>
    <TaskInput @addTask="addTask"/>
    <TaskList/>
  </div>
</template>

<script>
import TaskList from './components/TaskList'
import TaskInput from './components/TaskInput'

export default {
  name: 'app',
  components: {
    TaskList,
    TaskInput
  },
  data() {
    return {
      tasks: []
    }
  },
  mounted() {
    if (localStorage.getItem("tasks"))
      this.tasks = JSON.parse(localStorage.getItem("tasks"));
  },
  methods: {
    addTask(task) {
      this.tasks.push(task);
      localStorage.setItem("tasks", JSON.stringify(this.tasks));
    }
  }
}
</script>

<style lang="scss">
  .container {
    max-width: 600px;
  }
</style>
