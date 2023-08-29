<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="warpper bg-[#f4f4f4] py-12 px-[4rem]">
    <h1 class="text-3xl">Applications</h1>

    <div class="whole-container flex py-[5rem] px-8">
        <div class="left-container flex flex-wrap">
            <div class="content">
                <img src="../../assets/images/icon/medal.png" alt="">
                <h2>E-mobility</h2>
                <p>Lorem, ipsum dolor.</p>
            </div>
            <div class="content">
                <img src="../../assets/images/icon/honest.png" alt="">
                <h2>Power tools</h2>
                <p>Lorem, ipsum dolor.</p>
            </div>
            <div class="content">
                <img src="../../assets/images/icon/support.png" alt="">
                <h2>Energy storage stystem</h2>
                <p>Lorem, ipsum dolor.</p>
            </div>
            <div class="content">
                <img src="../../assets/images/icon/administration.png" alt="">
                <h2>Industrial power equipment</h2>
                <p>Lorem, ipsum dolor.</p>
            </div>
        </div>
        <div class="right-container w-[30rem]">
            <img src="../../assets/images/application.png" alt="">
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

.content {
    width:calc(50% - 1rem);
    border-left:2px solid #00f641;
    padding-left:2rem;
    margin-bottom:2rem;
    display:flex;
    flex-direction: column;
    justify-content: space-between;
}

.content > img {
    width:5rem;
}

.content > h2 {
    font-weight: bold;
    padding-top:1rem;
}




</style>