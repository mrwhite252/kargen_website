<template>
    <div class="warpper py-8 px-[4rem] relative">
      <h1 class="text-4xl">Our Values</h1>
      <img class="absolute w-[25rem] bottom-16 left-0" src="../../assets/images/our-values.png" alt="">
      <div class="whole-container flex py-[3rem] px-8 justify-between">
        <div class="ml-auto w-[35%] flex flex-grow justify-center items-center  ">
        </div>  
        <div class="w-[60%] mr-auto flex flex-wrap mt-8">
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
      margin-bottom:5rem;
      display:flex;
      flex-direction: column;
      justify-content: center;
  }
  
  .content > img {
      width:4rem;
  }
  
  .content > h2 {
      font-weight: bold;
      padding-top:1rem;
  }
  
  
  
  
  </style>