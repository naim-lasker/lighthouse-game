<template>
  <div class="d-flex justify-content-between px-3 py-3">
    <div class="d-flex">
      <div class="mr-3">
        <img src="../assets/images/wallet.png" alt="Wallet">
      </div>

      <div class="wallet-left">
        <div class="d-flex">
          <h5 class="m-0 title">KEN</h5>
          <img class="mx-2" src="../assets/images/crown.png" alt="Crown">
          <h5 class=" m-0">7</h5>
        </div>

        <div>
          <h5 class="m-0"><small class="title">$</small>122131231</h5>
        </div>
      </div>
    </div>

    <div class="wallet-center">
      <img src="../assets/images/line.png" alt="Line">
    </div>
    
    <div class="wallet-right">
      <p class="m-0">
        <img src="../assets/images/sound.png" alt="Wallet">
        <span class="ml-2">:Dragon Boat Festival holiday!holiday!holiday!holiday!Drago</span>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style scoped>
.wallet-left .title {
  color: #979797;
  font-weight: 400;
}

.wallet-center img {
  height: 60px;
}
.wallet-right {
  max-width: 180px;
  font-size: 15px;
  color: #979797;
  word-wrap: break-word;
}
</style>
