

<template>

<div class="relative">
  <Navbar/>
  <Welcome/>
  <DescSection/>
  <SwipeCards/>
  <Achievement/>
  <ProductIntro/>
  <Application/>
  <LatestNews/>
  <PageFooter/>
</div>


</template>


<script setup>
import Welcome from '../components/homepageComponents/Welcome.vue';
import DescSection from "../components/homepageComponents/DescSection.vue";
import SwipeCards from "../components/homepageComponents/SwipeCards.vue";
import Achievement from "../components/homepageComponents/Achievement.vue";
import ProductIntro from "../components/homepageComponents/ProductIntro.vue";
import Application from "../components/homepageComponents/Application.vue";
import LatestNews from '../components/homepageComponents/LatestNews.vue';
import Navbar from '../components/Navbar.vue';
import PageFooter from '../components/PageFooter.vue';



</script>