<template>
  <div id="app">
    <Menur60_Header />
    <Menur60_HeroSection />
    <router-view/>
  </div>
</template>

<script>
  import Menur60_Header from './components/Menur60_Header.vue';
  import Menur60_HeroSection from './components/Menur60_HeroSection.vue';

  export default {
    components: {
      Menur60_Header,
      Menur60_HeroSection,
    },
  };
</script>

<style>

</style>
