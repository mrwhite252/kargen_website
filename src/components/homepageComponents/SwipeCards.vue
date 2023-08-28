<template>


<div class="wrapper">

    <h1 class="text-center text-2xl py-8 text-[#3e54d1]">Trusted by businesses worldwide</h1>


    <Swiper class="swpier"
    :slides-per-view="6"
        :space-between="50"
        :navigation="true"
        :modules="modules"
        @swiper="onSwiper"
        @slideChange="onSlideChange"
    >
        <SwiperSlide>
            <img src="../../assets/images/swipeLogo/benz.png" alt="">
        </SwiperSlide>
        <SwiperSlide class="swiper-slide" ><img src="../../assets/images/swipeLogo/nio.png" alt=""></SwiperSlide>
        <SwiperSlide class="swiper-slide"><img src="../../assets/images/swipeLogo/byd.png" alt=""></SwiperSlide>
        <SwiperSlide class="swiper-slide"><img src="../../assets/images/swipeLogo/tesla.png" alt=""></SwiperSlide>
        <SwiperSlide class="swiper-slide"><img src="../../assets/images/swipeLogo/toyota.png" alt=""></SwiperSlide>
        <SwiperSlide class="swiper-slide"><img src="../../assets/images/swipeLogo/xpeng.png" alt=""></SwiperSlide>
    </Swiper>
</div>


</template>

<script>

import { Swiper, SwiperSlide } from 'swiper/vue';
import { Navigation } from 'swiper/modules';
// import { register } from 'swiper/element/bundle';
import 'swiper/css';
import 'swiper/css/navigation';


export default {

    components: {
        Swiper,
        SwiperSlide
    },

    setup() {

        // const swiperContainer = this.$refs.swiperRef;

        // const params = {
        //     navigation: true,

        //     injectStyles: [

        //     ]
        // }
       
        return {

            modules: [Navigation],
        }
    }

}
</script>

<style scoped>

.wrapper {
    width:100%;
    background-color:#eee;
}
.swiper {
    width:80%;
    margin: 0 auto;
    padding: 2rem 3rem;
}

/* .swiper-slide {
    border: 1px solid red;
} */





</style>