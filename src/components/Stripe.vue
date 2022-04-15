<template>
  <div>This is just a useless div with a prop named {{ name }}</div>
</template>

<script>
export default {
  name: "Stripe",
  props: ["name"],
};
</script>

<style scoped>
div {
  background-color: #bbbc11;
  padding: 4px;
  border-top: black 3px solid;
  border-right: black 13px solid;
}
div:hover {
  transform: skew(-20deg) translateX(10px);
}
</style>
