<template>
  <h1>Home Page</h1>
  <button @click="goAboutPage">About 페이지로 이동</button>
  <hr class="my-4" />
  <AppGrid :items="items" v-slot="{ item }">
    <AppCard>{{ item }}</AppCard>
  </AppGrid>
</template>

<script setup>
import { ref } from 'vue';
import { useRouter } from 'vue-router';
import AppCard from '@/components/AppCard.vue';
import AppGrid from '@/components/AppGrid.vue';
const router = useRouter();
const goAboutPage = () => {
  router.push('/about');
};
const items = ref(['사과', '딸기', '포도', '바나나']);
</script>
