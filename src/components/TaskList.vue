<template>
    <div>
        <h1>Task List</h1>
        <TaskItem/>
    </div>
</template>

<script>
    import TaskItem from './TaskItem'
    export default {
        name: 'TaskList',
        components: {
            TaskItem
        }
    }
</script>