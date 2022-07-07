<template>
  <div>
    <button id="clickMe" @click="clickMeClicked">Click Me!</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
    }
  },
  mounted() {
    let clickMe = document.getElementById('clickMe')
    clickMe.style.top = this.getRandomNumber(0, this.clientHeight - 50) + 'px'
    clickMe.style.left = this.getRandomNumber(0, this.clientWidth - 160) + 'px'
  },
  props: {
    clientWidth: Number,
    clientHeight: Number,
  },
  methods: {
    getRandomNumber(min, max) {
      return Math.random() * (max - min) + min
    },
    clickMeClicked() {
    },
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
