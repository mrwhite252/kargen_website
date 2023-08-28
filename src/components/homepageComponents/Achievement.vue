<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="wrapper flex justify-center py-20">

    <div class="content flex flex-col items-center px-16 py-8" v-for="content in contents" :key="content.id">
        <h1> {{ content.number }}</h1>
        <p> {{ content.message }}</p>
        <div></div>
    </div>
    
  </div>
</template>

<script setup>

const contents = [
    {
        number:'1800',
        message:'㎡ R&D center'
    },
    {
        number:'100',
        message:'papers'
    },
    {
        number:'1800',
        message:'㎡ plant'
    },
    {
        number:'50',
        message:'patents'
    },
]

</script>

<style scoped>

.wrapper {
    width:100%;
    background-image:url('../../assets/images/section-background.png');
    background-repeat: no-repeat;
    background-size: cover;
}


h1 {
    font-size: 3rem;
}

p {
    font-size: 1.2rem;
}

.content {
    border-top:0;
    border-left:0;
    border-bottom:0;
    border-right:2px;
    border-style: solid;
    border-image-slice: 2;
    border-image-source:  linear-gradient(to bottom,#3e54d1, #00f641);
}

.content:last-child {
    border-right:0;
}

</style>