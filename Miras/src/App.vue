<template>
  <div id="app">
    
    <Header />
    
    
    <Photo />
  </div>
</template>

<script setup>

import Header from './components/Header.vue';
import Photo from './components/Photo.vue';
</script>

<style>
#app {
  display: flex; 
  flex-direction: column; 
  align-items: center; 
  padding: 0 2rem; 
  max-width: 1280px; 
  margin: 0 auto; 
  font-weight: normal; 
  box-sizing: border-box; 
}


* {
  margin: 0;
  padding: 0;
  box-sizing: border-box; 
}

body {
  margin: 0;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
}
</style>
