<template>


<div class="wrapper">

    <h1 class="text-center text-2xl py-8 text-[#3e54d1]">Trusted by businesses worldwide</h1>

    <swiper-container class="swiper-container"
        :slides-per-view="3"
        :space-between="50"
        :loop="true"
        :centered-slides="false"
        :navigation="true">
      <swiper-slide class="swiper-slide" v-for="content in contents" :key="content.id" ><img :src="content.imgSrc" alt=""></swiper-slide>
    </swiper-container>

</div>


</template>

<script>

import {register} from 'swiper/element/bundle';



export default {

    components:{
    },

    data(){
        return {
            contents:[
                {
                    id:1,
                    imgSrc:'src/assets/images/swipeLogo/nio.png'
                },
                {
                    id:2,
                    imgSrc:'src/assets/images/swipeLogo/byd.png'
                },
                {
                    id:3,
                    imgSrc:'src/assets/images/swipeLogo/tesla.png'
                },
                {
                    id:4,
                    imgSrc:'src/assets/images/swipeLogo/toyota.png'
                },
                {
                    id:5,
                    imgSrc:'src/assets/images/swipeLogo/xpeng.png'
                },
            ],
    }
        },

        mounted() {
            register();
        }


    }
</script>

<style scoped>

.wrapper {
    width:100%;
    background-color:#eee;
}

.swiper-container {
    padding: 2rem;
}

.swiper-slide {
    padding:2rem;
}





</style>