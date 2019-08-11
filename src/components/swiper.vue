<template>
  <div class="block">
    <span class="demonstration">默认 Hover 指示器触发</span>
    <el-carousel>
      <el-carousel-item v-for="item in data" :key="item.cid">
        <div class="image" :style="{backgroundImage: `url(${imgurl + item.img})`}"></div>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<script>
export default {
    props: {
        data: {
            type: Array,
            default: () => []
        }
    }
}
</script>

<style scoped>
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
.image {
    width: 100%;
    height: 300px;
    background-repeat: no-repeat;
    background-position: center center;
    background-size: cover;
}
</style>