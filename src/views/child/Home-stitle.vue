<template>
  <div>
    <!-- 小型图片加文字导航栏1 -->
    <div class="home-stitle">
      <p>{{msg1}}</p>
      <span>{{msg2}}</span>
    </div>
    <!-- 小型图片加文字导航栏2 -->
  </div>
</template>
<script>
  export default {
    name: "Home-stitle",
    props: {
      msg1:{default:"特别推荐"},
      msg2:{default:"Special Offer"}
      
      
    },
    data() {
      return {
      }
    },
    methods: {

    },
    created() {

    }
  }
</script>
<style scoped>
.home-stitle{
  text-align: center;
    padding-top: 0.8rem;
    padding-bottom: 0.5rem
}
.home-stitle span{
  color: #9b7338;
    font-size: 13px;
    line-height: 24px;
    letter-spacing: 8px;
    font-family: Arial;
}
</style>