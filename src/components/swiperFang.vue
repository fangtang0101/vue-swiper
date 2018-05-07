<!-- https://github.com/surmon-china/vue-awesome-swiper -->
<!-- https://surmon-china.github.io/vue-awesome-swiper/ -->
<template>
  <div>
    <swiper :options="swiperOption">
      <swiper-slide>
        <div class="swiper-zoom-container">
          <img :src="url">
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="swiper-zoom-container">
          <img :src="url">
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="swiper-zoom-container">
          <img :src="url">
        </div>
      </swiper-slide>
      <div class="swiper-pagination swiper-pagination-white" slot="pagination"></div>
      <div class="swiper-button-prev" slot="button-prev"></div>
      <div class="swiper-button-next" slot="button-next"></div>
    </swiper>
  </div>
</template>
<script>
// import Swiper from 'vue-swiper'
import 'swiper/dist/css/swiper.css'
import { swiper, swiperSlide } from 'vue-awesome-swiper'

export default {
  components: {
    swiper,
    swiperSlide
  },
  name: 'sw',
  data() {
    return {
      url: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1525670746457&di=ee3a429c99d08fe3cca6c1531d724e79&imgtype=0&src=http%3A%2F%2Fpic2016.ytqmx.com%3A82%2F2016%2F1229%2F18%2F5.jpg%2521960.jpg',
      msg: 'Welcome to Your Vue.js App',
      swiperOption: {
        zoom: true,
        pagination: {
          el: '.swiper-pagination'
        },
        navigation: {
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev'
        }
      }
    }
  }
}

</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

</style>
