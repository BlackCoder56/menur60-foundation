<template>
  <div id="app">
    <Menur60_Header />
    <router-view/>
  </div>
</template>

<script>
  import Menur60_Header from './components/Menur60_Header.vue';
  
  export default {
    components: {
      Menur60_Header,
    },
  };
</script>

<style>

</style>
