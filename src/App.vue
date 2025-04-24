<script setup>
// import { RouterLink, RouterView } from 'vue-router'
import PortfolioView from './views/PortfolioView.vue'
import NavBar from '@/components/NavBar.vue'
</script>

<template>
  <NavBar />
  <PortfolioView />
</template>

<style>
#app {
  margin-top: 3rem;
  scroll-padding-top: 5rem;
}
</style>
