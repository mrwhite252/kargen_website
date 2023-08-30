<template>
  <div>
      <div class="grid grid-rows-2 grid-cols-4 grid-flow-col gap-x-8 gap-y-4 p-12">
        <div v-for="content in contents" :key="content.id" class="border-b pb-4">
            <h1 class="text font-bold pb-2">{{ content.title }}</h1>
            <p class="text-sm">{{ content.date }}</p>
            <img :src="content.imgSrc" alt="" class="w-[15rem] h-[10rem] my-6">
            <p>{{ content.desc }}</p>
        </div>
      </div>
      <div class="mx-auto py-8 rounded-xl w-[10rem]">
        <p class="btn-text">View More</p>
        </div>
  </div>
</template>

<script setup>

const contents = [
    {
        id:0,
        title:'Kargen on X Ceremony',
        date:'August 23 2023',
        imgSrc:'src/assets/images/news_1.jpeg',
        desc:'Lorem ipsum dolor sit amet td dlr Lorem ipsum dolor '
    },
    {
        id:1,
        title:'Lorem ipsum ipsum dolor sit amet',
        date:'August 23 2023',
        imgSrc:'src/assets/images/news_2.jpeg',
        desc:'Lorem ipsum dolor sit amet td dlr Lorem ipsum dolor '
    },
    {
        id:2,
        title:'Lorem ipsum ipsum dolor sit amet',
        date:'August 23 2023',
        imgSrc:'src/assets/images/news_3.jpeg',
        desc:'Lorem ipsum dolor sit amet td dlr Lorem ipsum dolor '
    },
    {
        id:3,
        title:'Kargen on X Ceremony',
        date:'August 23 2023',
        imgSrc:'src/assets/images/news_1.jpeg',
        desc:'Lorem ipsum dolor sit amet td dlr Lorem ipsum dolor '
    },
    {
        id:4,
        title:'Lorem ipsum ipsum dolor sit amet',
        date:'August 23 2023',
        imgSrc:'src/assets/images/news_2.jpeg',
        desc:'Lorem ipsum dolor sit amet td dlr Lorem ipsum dolor '
    },
    {
        id:5,
        title:'Lorem ipsum ipsum dolor sit amet',
        date:'August 23 2023',
        imgSrc:'src/assets/images/news_3.jpeg',
        desc:'Lorem ipsum dolor sit amet td dlr Lorem ipsum dolor '
    },
    {
        id:6,
        title:'Lorem ipsum ipsum dolor sit amet',
        date:'August 23 2023',
        imgSrc:'src/assets/images/news_1.jpeg',
        desc:'Lorem ipsum dolor sit amet td dlr Lorem ipsum dolor '
    },
    {
        id:7,
        title:'Kargen on X Ceremony',
        date:'August 23 2023',
        imgSrc:'src/assets/images/news_2.jpeg',
        desc:'Lorem ipsum dolor sit amet td dlr Lorem ipsum dolor '
    },

]

</script>

<style scoped>

.btn-text {
    background: linear-gradient(to right, #3e54d1, #00f641);
    border-radius: 20px;
    padding:0.5rem 1rem;
    color:white;
    text-align: center;
    cursor: pointer;
}

</style>