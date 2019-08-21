<template lang="pug">
h1(:class="{[$style.inv]: loaded}") Hello World
</template>

<script lang="ts">
import { Component, Vue } from "nuxt-property-decorator"

@Component
export default class IndexPage extends Vue {
  loaded = false

  mounted() {
    this.loaded = true
  }
}
</script>

<style lang="scss" module>
.inv {
  background-color: black;
  color: white;
}
</style>
