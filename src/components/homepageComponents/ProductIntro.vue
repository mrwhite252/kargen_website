<template>
  <div class="wrapper">

    <img class="mx-auto" src="../../assets/images/products.png" alt="">
    <div class="content-wrap flex justify-around py-12">
        <div>
            <img src="../../assets/images/icon/sphere.png" alt="">
            <p class="title">Polymer Microspheres</p>
        </div>
        <div>
            <img src="../../assets/images/icon/carbon-nanotube.png" alt="">
            <p class="title">Carbon Nanotubes</p>
        </div>
        <div class="flex flex-col">
            <img src="../../assets/images/icon/molecule.png" alt="">
            <p class="title">Metal Organic Frameworks</p>
            <div class="product-name">
                <p>KAR-M01</p>
                <p>|</p>
                <p>KAR-M16</p>
            </div>
            <div class="more-info">More</div>
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
    background-image: url('../../assets/images/productIntro-background.png');
    background-repeat: no-repeat;
    background-size: cover;
}

.content-wrap img {
    width: 6rem;
    margin:2rem 4rem;
}

.content-wrap p {
    font-size:1.2rem;
    color:white;
}

.title {
    border-bottom: 1px solid white;
    padding: 1rem;
    margin-bottom:1.5rem;
    text-align: center;
}

.product-name {
    margin-bottom:1rem;
}

.more-info {
    border:1px solid white;
    border-radius: 20px;
    cursor: pointer;
    color:white;
    width:50%;
    padding:0.5rem 1rem;
    margin:0.5rem 0;
    text-align: center;
}





</style>