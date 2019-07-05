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
  }
}
</script>

<style lang="scss">
  .container {
    max-width: 600px;
  }
</style>
