<template>
  <div>
    <!-- 首页头部1 -->
    <div class="header-title">
      <ul>
        <li class="header-item w-25">
          <a href="javascript:;">
            <img src="img/appimg/ia_100000001.png" class="simg" style="padding:0 0.3rem">
          </a>
        </li>
        <li class="header-item w-50 " style="text-align:center">
          <a href="javascript:;">
            <img src="img/appimg/ia_100000002.png" class="mlogo">
          </a>
        </li>
        <li class="header-item w-25 fl">
          <a href="javascript:;">
            <img src="img/appimg/ia_100000003.png" class="simg" style="padding:0 0.3rem">
          </a>
          <a href="javascript:;">
            <img src="img/appimg/ia_100000004.png"  class="simg" style="padding:0 0.3rem">
          </a>
        </li>
      </ul>
      <div class="clearfix"></div>
    </div>
    <!-- 首页头部2 -->
  </div>
</template>
<script>
  export default {
    name: "Home-header",
    props: {
      msg: {
        default: ""
      }
    },
    data() {
      return {}
    },
    methods: {

    },
    created() {

    }
  }
</script>
<style scoped>

  .header-title {
   width: 100%;
    height: 45px;
    line-height: 45px;
    background-color: #fff;
  }
  ul{
    list-style:none;
  }
   .header-title ul li{
     float: left;
   }
.fl{
  text-align: right;
}
   .w-25{
     width:25%!important;
   }
   .w-50{
     width:50%!important;
   }
  .header-title ul .header-item a{
    /* display:inline-block; */
    text-align: center;
    line-height: 45px;
  }
  .header-title ul .header-item img{
    max-width: 50%;
    max-height: 45px;
    vertical-align: middle;
    display:inline-block;
  }
 .header-title ul .header-item .mlogo{
    max-width: 100%;
 }
 @media screen and (max-width: 500px) {
   .simg{
     width: 30%;
    max-height: 45px;
 }
}
 
</style>