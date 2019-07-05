<template>
    <div>
        <div class="form-group">
            <input
                type="text"
                class="form-control"
                placeholder="Enter a New Task"
                @keyup.enter="addTask($event)"
            >
        </div>
    </div>
</template>

<script>
    export default {
        methods: {
            addTask(event) {
                if (event.target.value === "") return;
                this.$emit("addTask", {
                    title: event.target.value,
                    completed: false
                });
                event.target.value = "";
            }
        }
    }
</script>