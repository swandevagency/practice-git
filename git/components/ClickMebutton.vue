<template>
  <div>
    <button id="clickMe">Click Me!</button>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
  props: {
    clientWidth: Number,
    clientHeight: Number,
  },
}
</script>

<style>
button {
  position: relative;
  color: white;
  padding: 13px 26px;
  background-color: rgb(97, 95, 95);
  border: 1px solid rgb(97, 95, 95);
  box-shadow: 0 0 16px rgba(0, 0, 0, 0.5);
  border-radius: 8px;
  cursor: pointer;
}
</style>
