<template>
  <div :class="[task.reminder ? 'reminder' : '', 'task']">
    <h3>
      {{ task.text }}
      <i class="fas fa-times"></i>
    </h3>
    <p>{{ task.day }}</p>
  </div>
</template>
;

<script>
export default {
  name: "Task",
  props: {
    task: Object,
  },
};
</script>

<style scoped>
.fas {
}

.reminder {
  border-left: 5px green solid;
}

.task {
  width: 90%;
}
</style>
