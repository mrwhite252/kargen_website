<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="wrapper">

    <div class="relative w-[80%] mx-auto">
    <div class="text-wrapper">
        <h1 class="pb-4" >Eco-friendly solution for<br/>
            lithium-ion energy<br/>
            storage system</h1>
            <p class="pb-4">Create a sustainable world by innovative material tech</p>
            <div class="playVidBtn">
                <img src="../../images/trangle.png" alt="">
                <p>Watch Video</p>
            </div>
    </div>

    </div>
   
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

.wrapper {
    height:30rem;
    width: 100%;
    background-image:url('../../images/background-1.png'),linear-gradient(-120deg, #3e54d1, #00f641);
    background-repeat: no-repeat;
    background-size:70% auto,auto auto;
    background-position: 8rem 5rem, 0;
    padding-top:4rem;
    padding-left:0;
    padding-right:10rem;
}

h1 {
    font-size: 2rem;
}

@media screen and (min-width: 1028px) {
    .wrapper {
        height:35rem; 
    }
}
@media screen and (min-width: 1300px) {
    .wrapper {
        background-size:65% auto,auto auto;
        background-position: 12rem 2rem, 0;
    }

    h1 {
        font-size: 2.5rem;
    }

    p {
        font-size: 1.2rem;
    }
}
@media screen and (min-width: 1400px) {
    .wrapper {
        height: 45rem;
        background-size:60% auto,auto auto;
        background-position: 12rem 5rem, 0;
        padding-top:6rem;
    }

    h1 {
        font-size: 2.8rem;
    }

    p {
        font-size: 1.2rem;
    }
}
.text-wrapper {
    padding:4rem;
    /* background: rgba(255,255,255,0.1); */
}

h1,p {
    color:white;
}

.playVidBtn {
    border: 1px solid white;
    border-radius: 2rem;
    display: flex;
    align-items: center;
    justify-content: space-around;
    width:10rem;
    padding:0.5rem 1rem;
}

.playVidBtn > img{
    width:1rem;
    display: block;
}

</style>