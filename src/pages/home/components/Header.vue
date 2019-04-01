<template>
  <div class="home-header">
    <img class="home-logo" src="@/assets/images/home/logo.png" alt="东莞中创智能制造系统有限公司">
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="scss" scoped>
$background:#0063BD;
.home-header {
  background: $background;
  color: #fff;
  .home-logo {
    margin: .2rem;
    width: 95%;
  }
}
</style>
