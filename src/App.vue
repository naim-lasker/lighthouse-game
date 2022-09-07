<template>
  <div class="main-container">
    <Header msg="Header"/>
    <Banner msg="Banner"/>
    <HotGame msg="HotGame"/>
    <Wallet msg="Wallet"/>
    <Features msg="Features"/>
    <Footer msg="Footer"/>
  </div>
</template>

<script>
import './assets/scss/_app.scss'

import Header from './layouts/Header'
import Banner from './components/Banner'
import HotGame from './components/HotGame'
import Wallet from './components/Wallet'
import Features from './components/Features'
import Footer from './layouts/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Banner,
    HotGame,
    Wallet,
    Features,
    Footer,
  }
}
</script>

<style scoped>
.main-container {
  margin: auto;
  max-width: 700px;
  background-color: #000;
}
</style>
