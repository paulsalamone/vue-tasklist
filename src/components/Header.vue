<template>
  <header>
    <h1>{{ title }}</h1>
    <div>
      <Button content="add task" color="#ffcf04" />
    </div>
  </header>
</template>

<script>
import Button from "./Button";
export default {
  name: "Header",
  components: {
    Button,
  },
  props: {
    title: String,
  },
};
</script>

<style scoped>
header {
  padding: 10px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  /* margin-bottom: 20px; */
}

h1 {
  /* text-align: center; */
}
</style>
