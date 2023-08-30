<template>
  <div class="px-12 py-16">
    <div class="titles text-center pb-12">
        <h1 class="text-4xl font-bold pb-4">We're Hiring!</h1>
        <p class="text-[#b0b0b0]">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
    </div>
    <div class="">
        <div class="content-container py-4 border-b-2 " v-for="content in contents" :key="content.id">
            <div class="show flex items-center">
                <div class="left-part">
                    <h2 class="text-2xl font-bold pb-2">{{ content.title }}</h2>
                    <p><span class="font-bold">Location:</span> {{ content.location }}</p>
                </div>
                <div class="ml-auto" @click="showContent">
                    <p class="text-4xl text-[#3f54d0]">+</p>
                </div>
            </div>
            <div v-if="showDesc">{{ content.desc }}</div>
        </div>
    </div>
  </div>
</template>

<script setup>

import { ref } from 'vue';

const contents = [
    {
        id:0,
        title:'Junior Product Manager',
        location:'ZHuhai, Shenzhen, Shanghai',
        desc:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio rem illo, nam excepturi odio aliquid? Optio tempore aliquam voluptate eius at dolorum voluptatem eaque accusantium!'
    },
    {
        id:1,
        title:'Senior Product Manager',
        location:'ZHuhai, Shenzhen, Shanghai',
        desc:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio rem illo, nam excepturi odio aliquid? Optio tempore aliquam voluptate eius at dolorum voluptatem eaque accusantium!'
    },
    {
        id:2,
        title:'Designer',
        location:'ZHuhai',
        desc:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio rem illo, nam excepturi odio aliquid? Optio tempore aliquam voluptate eius at dolorum voluptatem eaque accusantium!'
    },
    {
        id:3,
        title:'Product Manager',
        location:'Shenzhen, Shanghai',
        desc:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio rem illo, nam excepturi odio aliquid? Optio tempore aliquam voluptate eius at dolorum voluptatem eaque accusantium!'
    },
    {
        id:4,
        title:'Developer',
        location:'Shenzhen, Shanghai',
        desc:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio rem illo, nam excepturi odio aliquid? Optio tempore aliquam voluptate eius at dolorum voluptatem eaque accusantium!'
    },
]

let showDesc = ref(false);

const showContent = (e) => {
    console.log(e.target);
   return showDesc.value = !showDesc.value;
}


</script>


<style scoped>



</style>