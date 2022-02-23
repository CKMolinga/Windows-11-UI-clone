<template>
  <div>
    <app-home></app-home>
  </div>
</template>

<script>
import Home from "./components/Home.vue"

export default {
  components: {
    "app-home": Home,
  }
}
</script>

<style lang="scss">
*{
  box-sizing: border-box;
  margin: 0;
}
</style>
