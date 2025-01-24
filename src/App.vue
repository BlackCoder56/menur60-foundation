<template>
  <div id="app">
    <Menur60_Header />
    <Menur60_HeroSection />
    <Menur60_About />
    <Menur60_Projects />
    <Menur60_Contact />
    <Menur60Footer />
    <router-view/>
  </div>
</template>

<script>
  import Menur60_Header from './components/Menur60_Header.vue';
  import Menur60_HeroSection from './components/Menur60_HeroSection.vue';
  import Menur60_About from './components/Menur60_About.vue';
  import Menur60_Projects from './components/Menur60_Projects.vue';
  import Menur60_Contact from './components/Menur60_Contact.vue';
  import Menur60Footer from './components/Menur60Footer.vue';




  export default {
    components: {
      Menur60_Header,
      Menur60_HeroSection,
      Menur60_About,
      Menur60_Projects,
      Menur60_Contact,
      Menur60Footer,
    },
  };
</script>

<style>

</style>
