<!-- eslint-disable vue/multi-word-component-names -->
<template>
        <div class="flex justify-between h-[5rem] items-center fixed w-[80%] mx-auto left-0 right-0">
            <img class="w-[2rem]" src="../../images/logo_white.png" alt="">
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

}
</script>

<style scoped>

.router {
    padding-right: 1rem;
}

</style>