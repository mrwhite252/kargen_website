<!-- eslint-disable vue/multi-word-component-names -->
<template>
        <div v-bind="nvaBarColor" class="flex justify-between h-[5rem] items-center absolute px-16 mx-auto left-0 right-0">
            <router-link to="/"><img class="w-[2rem]" src="../assets/images/logo_white.png" alt=""></router-link>
            <ul class="flex justify-between">
                <router-link class="router" to="/about">About</router-link>
                <router-link class="router" to="/products">Products</router-link>
                <router-link class="router" to="/news">News</router-link>
                <router-link class="router" to="/resources">Resources</router-link>
                <router-link class="router" to="/contact">Contact</router-link>
            </ul>
            <div class="flex justify-around w-16 items-center">
                <img class="w-6 mr-4" src="../assets/images/global.png" alt="">
                <p class="text-white">English</p>
            </div>
        </div>
  
</template>

<script>

export default {
    computed:{
        nvaBarColor() {
            const routeName = this.$route.path;

            switch(routeName) {
                case '/':
                    console.log('home page');
                break;
                case '/about':
                    console.log('about page');
                break;
                case '/products':
                    console.log('products page');
                break;
                case '/news':
                    console.log('news page');
                break;
                case '/resources':
                    console.log('resource page');
                break;
                case '/contact':
                    console.log('contact page');
                break;
                default:
                    console.log('this somewhere else')
            }
            return null;
        }
    }
}




</script>

<style scoped>

.router {
    padding-right: 2rem;
    padding-left:2rem;
    line-height: 1;
    color:white;
    border-right:1px solid white;
}

.router:last-child {
    border-right: 0;
}

</style>