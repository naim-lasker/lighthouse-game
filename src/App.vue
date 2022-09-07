<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <Header msg="Header"/>
  <Banner msg="Banner"/>
  <Wallet msg="Wallet"/>
  <HotGame msg="HotGame"/>
  <Footer msg="Footer"/>
</template>

<script>
import './assets/scss/app.scss'

import Header from './layouts/Header'
import Banner from './components/Banner'
import Wallet from './components/Wallet'
import HotGame from './components/HotGame'
import Footer from './layouts/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Banner,
    Wallet,
    HotGame,
    Footer,
  }
}
</script>
