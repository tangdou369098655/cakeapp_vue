<template>
  <div class="home">
    <Swiper :data="data.carouselItems"/>
  </div>
</template>

<script>
import Swiper from '@/components/swiper'
export default {
  name: 'home',
  components: { Swiper },
  data() {
    return {
      data: {}
    }
  },
  mounted() {
    this.getData()
  },
  methods: {
    getData() {
      this.axios('/index/all').then(data => {
        this.data = data
      })
    }
  }
}
</script>