<template>
  <div id="app" class="container">
    <header>
      <div id="nav">
        <router-link to="/">Home</router-link> | 
        <router-link to="/about">About</router-link> 
      </div>
    </header>
    
    <main>
      <router-view :key="$route.fullPath"/>
    </main>
    
  </div>
</template>
<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class App extends Vue {}
</script>


<style lang="scss">
@import '@/scss/style.scss';
</style>
