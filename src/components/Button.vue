<template>
  <button @click="onClick()" :style="{ background: color }">
    {{ content }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    content: String,
    color: String,
  },
  methods: {
    onClick() {},
  },
};
</script>

<style scoped></style>
