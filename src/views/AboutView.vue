<script setup>
import { useRouter } from 'vue-router';
const router = useRouter();
const goHomePage = () => router.push('/');
</script>
<template>
  <h1>About Page</h1>
  <button @click="goHomePage">Home</button>
</template>
