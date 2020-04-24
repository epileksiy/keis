<template lang="pug">
  div
    Header
    Footer
</template>

<script>
import Footer from '../components/footer.vue'
import Header from '../components/header.vue'
export default {
  components: {
      Footer, Header
  }
}
</script>

<style>
@font-face {
  font-family: "Proxima Nova";
  src: url("../assets/fonts/ProximaNovaLight.ttf") format("truetype");
  font-style: normal;
  font-weight: normal;
}
</style>

