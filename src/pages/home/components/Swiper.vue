<template>
  <div>
    <div class="block">
      <el-carousel height="150px" :interval="5000" type="card" arrow="always">
        <el-carousel-item v-for="item in imgs" :key="item.id">
          <img :src="item.imgUrl" alt="{item.alt}" />
        </el-carousel-item>
      </el-carousel>
    </div>
    <div class="block">
      <span class="demonstration">Click 指示器触发</span>
      <el-carousel trigger="click" height="150px">
        <el-carousel-item v-for="item in 4" :key="item">
          <h3>{{ item }}</h3>
        </el-carousel-item>
      </el-carousel>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      imgs: [{'id': 1, 'imgUrl': '../../../../assets/images/home/2018120610413871.jpg', 'alt': '01'}, {'id': 2, 'imgUrl': 'Image/home/2018120616095421.jpg', 'alt': '02'}, {'id': 2, 'imgUrl': 'Image/home/2019012415262684.jpg', 'alt': '03'}]
    }
  }
}
</script>

<style lang="scss" scoped>
 .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 150px;
    margin: 0;
  }
  .el-carousel__item:nth-child(2n) {
     background-color: #99a9bf;
  }
  .el-carousel__item:nth-child(2n+1) {
     background-color: #d3dce6;
  }
</style>
