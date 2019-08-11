<template>
  <div>
    <!-- 小型图片加文字导航栏1 -->
    <div class="home-nav">
      <ul class="home-nav-all">
        <li class="home-nav-item" v-for="(item,i) in titleList" :key="i">
          <router-link :to="{path:'/product',query:{sid:i+1}}">
            <img :src='imglist[i]' alt="">
            <p>{{item}}</p>
          </router-link>
        </li>
      </ul>
      <div class="clear:both"></div>
    </div>
    <!-- 小型图片加文字导航栏2 -->
  </div>
</template>
<script>
  export default {
    name: "Home-snav",
    props: {
      
      
    },
    data() {
      return {
        titleList:['爱情鲜花','生日鲜花','道歉鲜花','进口鲜花','韩式鲜花','花束鲜花','高端鲜花','开业花篮','永生花','更多'] ,
       imglist:[
         'img/appimg/ia_100000009.png',
         'img/appimg/ia_100000010.png',
         'img/appimg/ia_100000011.png',
         'img/appimg/ia_100000012.png',
         'img/appimg/ia_100000013.png',
         'img/appimg/ia_100000014.png',
         'img/appimg/ia_100000015.png',
         'img/appimg/ia_100000016.png',
         'img/appimg/ia_100000017.png',
         'img/appimg/ia_100000018.png',
       
       ] 
      }
    },
    methods: {

    },
    created() {

    }
  }
</script>
<style scoped>
/* ul>li{
  list-style:none;
}
ul>li{
  float: left;
} */
.home-nav {
 padding:0.7rem 0;
}
.home-nav-all{
  display:flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}
.home-nav .home-nav-item{
width:20%;
text-align: center;
margin-bottom:0.5rem;
}
.home-nav .home-nav-item a img{
width:41px;
height:41px;
margin-bottom: 0.15rem;
display:inline-block;

}
.home-nav .home-nav-item a p{
  font-size:0.5rem;
}
</style>