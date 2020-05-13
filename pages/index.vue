<template lang="pug">
  div
    Header
    Hypno
    .a
      a There`s no bugs here
    Footer
</template>

<script>
import Footer from '../components/footer.vue'
import Header from '../components/header.vue'
import Hypno from '../components/hypno.vue'
export default {
  components: {
      Footer, Header, Hypno
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
  .a {
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: Proxima Nova;
    font-style: normal;
    font-weight: 600;
    font-size: 20px;;
  }
</style>

