<script setup>
import TheNav from './components/TheNav.vue';
</script>

<template>
  <TheNav></TheNav>

  <main>
    <RouterView></RouterView>
  </main>
</template>

<style>
@import './assets/base.css';
</style>
