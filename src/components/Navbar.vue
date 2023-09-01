<!-- eslint-disable vue/multi-word-component-names -->
<template>
        <div v-bind="nvaBarColor" class="flex justify-between h-[5rem] items-center absolute px-16 mx-auto left-0 right-0" :class="[hasBackGroundColor ? 'bg-[#f4f4f4]' : '']">
            <router-link to="/"><img class="w-[2rem]" :src="[whiteColor ? whiteLogo : blueLogo]" alt=""></router-link>
            <ul class="flex justify-between">
                <router-link class="router" :class="{white: whiteColor}"  to="/about"><p>About</p></router-link>
                <router-link class="router" :class="{white: whiteColor}"  to="/products"><p>Products</p></router-link>
                <router-link class="router" :class="{white: whiteColor}"  to="/news"><p>News</p></router-link>
                <router-link class="router" :class="{white: whiteColor}"  to="/resources"><p>Resources</p></router-link>
                <router-link class="router" :class="{white: whiteColor}"  to="/contact"><p>Contact</p></router-link>
            </ul>
            <div class="flex justify-around w-16 items-center">
                <img class="w-6 mr-4" :src="[whiteColor ? whiteIcon : blueIcon]" alt="">
                <p :class="[ whiteColor ? 'text-white' :'text-[#3e54d1]'  ]" >English</p>
            </div>
        </div>
  
</template>

<script>

export default {

    data() {
        return {
            whiteColor:false,
            hasBackGroundColor:false,
            whiteLogo:'src/assets/images/logo_white.png',
            blueLogo:'src/assets/images/logo_blue.png',
            whiteIcon:'src/assets/images/icon/internet.png',
            blueIcon:'src/assets/images/icon/internet2.png',
        }
    },

    computed:{
        nvaBarColor() {
            const routeName = this.$route.path;

            switch(routeName) {
                case '/':
                    console.log('home page');
                    // eslint-disable-next-line vue/no-side-effects-in-computed-properties
                    this.whiteColor = true;
                break;
                case '/about':
                    console.log('about page');
                break;
                case '/products':
                    console.log('products page');
                break;
                case '/news':
                    console.log('news page');
                    // eslint-disable-next-line vue/no-side-effects-in-computed-properties
                    this.hasBackGroundColor = true;
                break;
                case '/resources':
                    console.log('resource page');
                break;
                case '/contact':
                    console.log('contact page');
                    // eslint-disable-next-line vue/no-side-effects-in-computed-properties
                    this.hasBackGroundColor = true;
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
    color: #3e54d1;
    border-right:1px solid #3e54d1;
}

.white {
    color: white;
    border-right:1px solid white;
}

.router:last-child {
    border-right: 0;
}

a > p {
    line-height: 2;
}

a.router-link-active > p {
    line-height:2;
   border-bottom: 2px solid #00f641;
}


</style>