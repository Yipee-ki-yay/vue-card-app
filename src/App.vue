<template>
  <dir>
    <app-header></app-header>
    <app-content></app-content>    
  </dir>
</template>

<script>
  import AppHeader from './components/Header.vue';
  import AppContent from './components/Content.vue'; 

  export default {
    components: {
      AppHeader,
      AppContent,
    }
  }
</script>

<style>

</style>
