<template>
  <div class="footer d-flex justify-content-between align-items-center px-sm-5 px-3 py-3 mb-4">
    <img role="button" src="../assets/images/footer/home.png" alt="Home">
    <img role="button" src="../assets/images/footer/gift.png" alt="Gift">
    <img role="button" src="../assets/images/footer/money.png" alt="Money">
    <img role="button" src="../assets/images/footer/chat.png" alt="Chat">
    <img role="button" src="../assets/images/footer/user.png" alt="User">
  </div>
</template>

<script>
export default {
  name: 'FooterComp',
}
</script>

<style scoped>
  .footer {
    border-top-left-radius: 15px;
    border-top-right-radius: 10px;
    background-color: #1A1A1A;
  }

  @media screen and (max-width: 480px) {
    .footer img {
      width: 30px;
    }
  }

  @media screen and (max-width: 380px) {
    .footer img {
      width: 20px;
    }
  }
</style>
