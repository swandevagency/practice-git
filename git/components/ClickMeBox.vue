<template>
  <div id="box">
    <ClickMeButton :client-width="clientWidth" :client-height="clientHeight" />
    <div id="history">
      <ul>
        <History />
      </ul>
    </div>
  </div>
</template>

<script>
import ClickMeButton from '../components/ClickMeButton.vue'
import History from './History.vue'
export default {
  data() {
    return {
      clientWidth: 0,
      clientHeight: 0,
    }
  },
  mounted() {
    const box = document.getElementById('box')
    this.clientWidth = box.clientWidth
    this.clientHeight = box.clientHeight
  },
  components: {
    ClickMeButton,
    History,
  },
}
</script>

<style scoped>
#box {
  height: 28rem;
  border: 1px solid rgb(236, 236, 236);
  box-shadow: 0 0 16px rgba(109, 109, 109, 0.2);
  border-radius: 12px;
}

#history {
  position: relative;
  top: 630px;
}
</style>
