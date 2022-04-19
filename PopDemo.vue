<template>
  <section>
    component
  </section>
</template>

<script>
const componentConfig = {
  setup() {
  }
}

export default componentConfig;

export const showPopup = () => {
  // in dev mode, componentConfig.render exist
  // in build mode, componentConfig.render not exist
  // this issue happened from @vitejs/plugin-vue@1.8.1
  console.log("componentConfig'props ", Object.getOwnPropertyNames(componentConfig))
  alert("PopDemo.vue config'props >> " + Object.getOwnPropertyNames(componentConfig).join(", "))
}
</script>