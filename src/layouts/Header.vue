<template>
  <div class="header py-1 d-flex justify-content-between align-items-center mx-3 mx-sm-4">
    <img class="bell" role="button" src="../assets/images/bell.png" alt="Bell">
    <img class="logo" role="button" src="../assets/images/logo.png" alt="Logo">
    <img class="menu" role="button" src="../assets/images/menu.png" alt="Menu">
  </div>
</template>

<script>
export default {
  name: 'HeaderComp',
}
</script>

<style scoped>

  @media screen and (max-width: 480px) {
    .header .bell {
      width: 30px;
    }
    .header .logo {
      width: 140px;
    }
    .header .menu {
      width: 30px;
    }
  }

  @media screen and (max-width: 380px) {
    .header .bell {
      width: 20px;
    }
    .header .logo {
      width: 100px;
    }
    .header .menu {
      width: 20px;
    }
  }
</style>