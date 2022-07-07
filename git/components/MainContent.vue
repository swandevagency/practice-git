<template>
  <div class="main-content-component-wrapper" id="mainContent">
    <ClickMeBox />
    <NameInput />
    <StartButton />
  </div>
</template>

<script>
import ClickMeBox from '../components/ClickMeBox.vue'
import NameInput from '../components/NameInput.vue'
import StartButton from '../components/StartButton.vue'
export default {
  data() {
    return {}
  },
  components: {
    ClickMeBox,
    NameInput,
    StartButton,
  },
}
</script>

<style scoped>
#mainContent {
  width: 76%;
  margin: 150px auto 100px auto;
}
</style>
