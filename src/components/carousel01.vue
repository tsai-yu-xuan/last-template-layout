<template>
  <swiper
    :spaceBetween="30"
    :centeredSlides="true"
    :loop="true"
    :autoplay="{
      delay: 2500,
      disableOnInteraction: false,
    }"
    :pagination="{
      clickable: true,
    }"
    :modules="modules"
    class="mySwiper"
  >
    <swiper-slide><v-img src="https://jo-zu-works.site/img/pc/jozu_topimg02.jpg"></v-img></swiper-slide>
    <swiper-slide><v-img src="https://jo-zu-works.site/img/pc/jozu_topimg01.jpg"></v-img></swiper-slide>
    <swiper-slide><v-img src="https://picsum.photos/1080/680/?random=3"></v-img></swiper-slide>
    <swiper-slide><v-img src="https://picsum.photos/1080/680/?random=10"></v-img></swiper-slide>
  </swiper>
</template>
<script>
  // Import Swiper Vue.js components
  import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
  import 'swiper/css';

  import 'swiper/css/pagination';
  // import required modules
  import { Autoplay, Pagination } from 'swiper/modules';

  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {
        modules: [Autoplay, Pagination],
      };
    },
  };
</script>
