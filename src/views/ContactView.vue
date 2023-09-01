<template>
    <div>
      <Navbar/>
      <ContactForm/>
      <MapView/>
      <FAQSection/>


      <PageFooter/>
    
    </div>
    </template>
    
    
    <script setup>
    
    import Navbar from '../components/Navbar.vue';
    import PageFooter from '../components/PageFooter.vue';
    import ContactForm from '../components/contactpageComponents/ContactForm.vue';
    import MapView from '../components/contactpageComponents/MapView.vue';
    import FAQSection from '../components/contactpageComponents/FAQSection.vue';
    
    
    
    </script>
    
    <style>
    
    </style>