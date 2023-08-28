

<template>

<div class="relative">
  <Navbar/>
  <Welcome/>
  <DescSection/>
  <SwipeCards/>
  <Achievement/>
</div>


</template>


<script setup>
import Welcome from '../components/homepageComponents/Welcome.vue';
import DescSection from "../components/homepageComponents/DescSection.vue";
import SwipeCards from "../components/homepageComponents/SwipeCards.vue";
import Achievement from "../components/homepageComponents/Achievement.vue";
import Navbar from '../components/Navbar.vue';



</script>