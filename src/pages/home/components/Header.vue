<template>
  <div class="home-header">
    <div class="home-left">左边</div>
    <div class="home-right">右边</div>
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
  display: flex;
  justify-content: space-between;
  box-sizing: border-box;
  margin: .2rem;
  height: 2rem;
  line-height: 2rem;
  background: $background;
  color: #fff;
  .home-left {
    margin-left: .5rem;
  }
  .home-right {
    margin-right: .5rem;
  }
}
</style>
