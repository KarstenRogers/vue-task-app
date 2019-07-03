<template>
  <div id="app">
    <TaskList/>
    <TaskInput/>
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

<style>

</style>
