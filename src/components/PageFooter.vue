<template>
  <div class="bg-[#f4f4f4] px-12 py-8 text-[#747474]">
    <div class="upper-part flex pb-16">
        <div class="pr-16">
            <h1>About Us</h1>
            <p>About Kargen</p>
            <p>News</p>
            <p>Careers</p>
        </div>
        <div>
            <h1>Products</h1>
            <p>Polymer Microspheres</p>
            <p>Carbon Nanotubes</p>
            <p>Metal Organic Frameworks</p>
        </div>
        <div class="ml-auto text-center">
            <h1>Connect with us</h1>
           <div class="flex justify-around pb-4">
            <img src="../assets/images/icon/wechat.png" alt="">
            <img src="../assets/images/icon/linkedin.png" alt="">
            <img src="../assets/images/icon/sina-weibo.png" alt="">
           </div>
           <p>We would love to hear from you.</p>
        </div>
    </div>

    <div class="lower-part flex pt-8 text-l text-[#747474] w-[50%] justify-between">
        <p>&#169;<span>2023</span> Kargen Inc.</p>
        <p>Terms of Use</p>
        <p>Privacy Policy</p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

h1 {
    font-size:1.5rem;
    padding-bottom:1rem;
    color:black;
}


.upper-part {
    border-bottom-width: 1px;
    border-bottom-style: solid;
    border-image-slice: 2;
    border-image-source:  linear-gradient(to right,#3e54d1, #00f641);
}

img {
    width:2rem;
}

</style>