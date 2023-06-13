<template>
    <div :key="task.id" v-for="task in tasks">
        <Task
            @toggle-reminder="$emit('toggle-reminder', task.id)"
            @delete-task="$emit('delete-task', task.id)"
            :task="task"
        />
    </div>
</template>

<script lang="js">
import Task from './Task';

export default {
    // eslint-disable-next-line
    name: 'Tasks',
    props: {
        tasks: Array,
    },
    components: {
        Task,
    },
    emits: ['delete-task', 'toggle-reminder']
};
</script>
