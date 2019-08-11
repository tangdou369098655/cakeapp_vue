<template>
     <ul class="f2_banner">
              <li class="f2_banner_item">
                <router-link :to="{path:'/Details',query:{fid:myhref}}">
                  <img :src="imgurl" alt="">
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
.f2_banner_item img{
width: 100%;
}
.f2_banner_item{
width: 100%;
float: left;
}
.f2_banner {
display:flex;
justify-content: space-between;
align-items: center;
width: 50%;
padding:0 0.2rem 0 0.2rem;
padding-bottom: 0;
box-sizing: border-box;
display:inline-block;
}
</style>


