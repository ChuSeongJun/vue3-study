<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();
const goAboutPage = () => router.push('/about');
</script>
<template>
  <h1>Home Page</h1>
  <button @click="goAboutPage">About 페이지로 이동</button>
</template>
