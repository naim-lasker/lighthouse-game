<template>
  <div class="d-flex justify-content-between px-3 py-3">
    <div class="d-flex">
      <div class="mr-3 wallet-icon-container">
        <img src="../assets/images/wallet.png" alt="Wallet">
      </div>

      <div class="wallet-left mb-sm-0 mb-4">
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

    <div class="wallet-center d-none d-sm-block">
      <img src="../assets/images/line.png" alt="Line">
    </div>
    
    <div class="wallet-right ml-3 ml-sm-0">
      <p class="m-0">
        <img src="../assets/images/sound.png" alt="Wallet">
        <span class="ml-2">:Dragon Boat Festival holiday!holiday!holiday!holiday!Drago</span>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'WalletComp',
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

@media screen and (max-width: 480px) {
    .wallet-icon-container img {
      width: 30px;
    }
    .wallet-left .title, .wallet-left h5 {
      font-size: 13px;
    }
    .wallet-right {
      font-size: 13px;
      min-width: 150px;
    }
  }

  @media screen and (max-width: 380px) {
    .wallet-icon-container img {
      width: 20px;
    }
    .wallet-left .title, .wallet-left h5 {
      font-size: 12px;
    }
    .wallet-right {
      font-size: 12px;
      min-width: 120px;
    }
  }
</style>
