<template>
  
  <div class="flex px-12 py-16">
    <div class="left w-2/5 text-5xl leading-loose p-8">
        Frequently Asked <br/>
        Questions(FAQ)

    </div>
    <div class="right w-3/5 flex flex-col gap-8 px-12">
        <div class="flex items-center border-b-2 pb-4" v-for="content in contents" :key="content.id">
          <h1 class="text-xl"> {{ content.question }}</h1>
          <div class="ml-auto">
                    <p class="text-4xl text-[#3f54d0]">+</p>
                </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {

  data(){
    return {
      contents:[
        {
          id:1,
          question:"As a vendor/client how do I XXX XXX XXX?",
          answer:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio magnam voluptate molestias quibusdam, laborum numquam accusantium ea neque, illum ullam ipsum ab quisquam earum suscipit. Quaerat ad qui beatae consequuntur'
        },
        {
          id:2,
          question:"As a vendor/client how do I XXX XXX XXX?",
          answer:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio magnam voluptate molestias quibusdam, laborum numquam accusantium ea neque, illum ullam ipsum ab quisquam earum suscipit. Quaerat ad qui beatae consequuntur'
        },
        {
          id:3,
          question:"As a vendor/client how do I XXX XXX XXX?",
          answer:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio magnam voluptate molestias quibusdam, laborum numquam accusantium ea neque, illum ullam ipsum ab quisquam earum suscipit. Quaerat ad qui beatae consequuntur'
        },
        {
          id:4,
          question:"As a vendor/client how do I XXX XXX XXX?",
          answer:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio magnam voluptate molestias quibusdam, laborum numquam accusantium ea neque, illum ullam ipsum ab quisquam earum suscipit. Quaerat ad qui beatae consequuntur'
        },
      ]
    }
  }

}
</script>

<style>

</style>