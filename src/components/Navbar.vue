<!-- eslint-disable vue/multi-word-component-names -->
<template>
        <div v-bind="nvaBarColor" class="flex justify-between h-[5rem] items-center absolute w-[80%] mx-auto left-0 right-0">
            <router-link to="/"><img class="w-[2rem]" src="../assets/images/logo_white.png" alt=""></router-link>
            <ul class="flex justify-between w-64 ">
                <router-link class="router" to="/about">About</router-link>
                <router-link class="router" to="/products">Products</router-link>
                <router-link class="router" to="/news">News</router-link>
                <router-link class="router" to="/resources">Resources</router-link>
                <router-link class="router" to="/contact">Contact</router-link>
            </ul>
            <div class="flex justify-around w-16 items-center">
                <img class="w-4 mr-4" src="../../images/global.png" alt="">
                <p class="">English</p>
            </div>
        </div>
  
</template>

<script>

export default {
    computed:{
        nvaBarColor() {
            if(this.$route.path === '/about') {
               return console.log('at about page')
            }
            return console.log('at home page')
        }
    }
}




</script>

<style scoped>

.router {
    padding-right: 1rem;
}

</style>