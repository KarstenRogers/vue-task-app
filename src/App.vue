<template>
  <div id="app">
    <TaskList/>
    <TaskItem/>
    <TaskInput/>
  </div>
</template>

<script>
import TaskList from './components/TaskList'
import TaskItem from './components/TaskItem'
import TaskInput from './components/TaskInput'

export default {
  name: 'app',
  components: {
    TaskList,
    TaskItem,
    TaskInput
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
