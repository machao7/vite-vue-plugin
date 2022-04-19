<template>
  <section>
    <button @click="pop">check component props</button>
    <h4>dev mode: props includes render</h4>
    <h4>build mode: props not includes render</h4>
  </section>
</template>

<script>
import { showPopup } from "./PopDemo.vue";

export default {
  setup() {
    return {
      pop() {
        showPopup()
      }
    }
  }
}
</script>