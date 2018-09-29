<template>
  <dir>
    <app-header :cnt="cnt"></app-header>
    <app-content
      @minus="onMinus"
      @plus="onPlus"
    ></app-content>
  </dir>
</template>

<script>
  import AppHeader from './components/Header.vue';
  import AppContent from './components/Content.vue'; 

  export default {
    data() {
        return {
            cnt: 1, 
        }
    },
    methods: {
      onMinus() {
        if(this.cnt > 1) {
          this.cnt--;
        }
      },
      onPlus() {
        this.cnt++;
      }
    },
    components: {
      AppHeader,
      AppContent,
    }
  }
</script>

<style>

</style>
