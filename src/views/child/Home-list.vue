<template>
     <ul class="f2_banner">
              <li>
                <router-link :to="{path:'/Details',query:{fid:myhref}}">
                  <img :src="imgurl" alt="">
                  <div>
                      <h3>{{title}}</h3>
                      <h2>￥{{price}}</h2>
                      <p>
                        APP折后￥
                        <span class="update_app_price">{{price-20}}</span>
                        元
                      </p>	
                  </div>
                </router-link>  
              </li>
            
            </ul>
</template>
<script>

    // import '../assets/css/base.css';
// import '../assets/js/index.js';
  export default{
    data(){
      return {
        
       
      }
      
    },
    props:{
        myhref:{default:""},
        imgurl:{default:""},
        price:{default:""},
        title:{default:""},
      },
    created(){
      
    }
  }

</script>
<style scoped>
.f2_banner{
  max-width: 33%;
display:flex;
justify-content: space-between;
align-items: center;
padding:0 0.1rem;
box-sizing: border-box;
display:inline-block;
}
/*鼠标悬浮图片移动效果*/
.f2_banner>li img:hover{
  transform: translateX(-10px);
}
.f2_banner>li img{
  max-width: 100%;
  overflow: hidden;
  transition: all 0.2s;
}
.f2_banner>li{
  float: left;
  max-width: 100%;
  cursor: pointer;
}
/*f2 div上内边距 文字居中 color 大小*/
.f2_banner>li div{
  text-align: center;
  padding-bottom: 0.8rem;
}
.f2_banner>li h3{
  font-size: 0.7rem;
  color: #555;
  height:30px;
  line-height: 30px;
  max-width: 100%;
  overflow: hidden;

}
.f2_banner>li h2{
 color: #9b7338;
  padding-top: 2px;
    font-size: 0.5rem;
}
.f2_banner>li p{
  -o-text-overflow: ellipsis;
  text-overflow: ellipsis;
      color: #9b7338;
    padding-top: 2px;
    font-size: 0.4rem;
}
</style>


