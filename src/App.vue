<template>
  <Header msg="Header"/>
  <Banner msg="Banner"/>
  <Wallet msg="Wallet"/>
  <HotGame msg="HotGame"/>
  <Features msg="Features"/>
  <Footer msg="Footer"/>
</template>

<script>
import './assets/scss/_app.scss'

import Header from './layouts/Header'
import Banner from './components/Banner'
import Wallet from './components/Wallet'
import HotGame from './components/HotGame'
import Features from './components/Features'
import Footer from './layouts/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Banner,
    Wallet,
    HotGame,
    Features,
    Footer,
  }
}
</script>
