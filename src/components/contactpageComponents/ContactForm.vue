<template>
  
  <div class="flex pt-[8rem] pl-[4rem]">
    <div class="left w-2/5">
        <div class="thumb">
            <h1 class="text-5xl pb-4">Contact Us</h1>
    <p>Let us know what you are interested in, or what you are looking for. We are here to help.</p>
        </div>
        <div class="form flex flex-col gap-8 mb-8 mt-4">
            <div class="first-line flex justify-between">
                <input type="text" name="" id="" placeholder="First name*">
                <input type="text" name="" id="" placeholder="Last Name*">
            </div>
            <div class="second-line flex justify-between">
                <input type="email" name="" id="" placeholder="Email*">
                <input type=" tel" name="" id="" placeholder="Phone*">
            </div>
            <div class="third-line flex justify-between">
                <input type="text" name="" id="" placeholder="Company*">
                <input type="text" name="" id="" placeholder="Job Title*">
            </div>
            <input class="h-20 text-left" type="textarea" name="" id="" placeholder="Tell us more*">
        </div>

        <div class="rounded-xl w-[8rem]">
        <p class="btn-text">Send</p>
        </div>

    </div>
    <div class="right w-3/5 flex justify-center items-center p-4">
        <img class="w-[80%]" src="../../assets/images/contact-thumb.png" alt="">
    </div>
   
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
input {
    box-sizing:border-box;
    border: 1px solid black;
    padding:0.5rem 1rem;
}

.btn-text {
    background: linear-gradient(to right, #3e54d1, #00f641);
    border-radius: 20px;
    padding:0.5rem 1rem;
    color:white;
    text-align: center;
    cursor: pointer;
}

</style>