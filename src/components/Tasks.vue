<template>
  <div :key="task.id" v-for="task in tasks" class="task-container">
    <Task :task="task" />
  </div>
</template>

<script>
import Task from "./Task.vue";
export default {
  name: "Tasks",
  props: {
    tasks: Array,
  },
  components: {
    Task,
  },
};
</script>

<style scoped>
.task-container {
  background-color: white;
  border: 1px solid lightblue;
  margin: 5px;
}
</style>
