<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();

const goPage = () => {
  router.push({
    name: 'PostCreate'
  });
};
</script>
<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Navbar</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav me-aute">
          <li class="nav-item">
            <RouterLink class="nav-link" active-class="active" to="/">Home</RouterLink>
          </li>
          <li class="nav-item">
            <RouterLink class="nav-link" active-class="active" to="/about">About</RouterLink>
          </li>
          <li class="nav-item">
            <RouterLink class="nav-link" active-class="active" :to="{ name: 'PostList', replace: true }"> 게시글 </RouterLink>
          </li>
          <li class="nav-item">
            <RouterLink class="nav-link" active-class="active" to="/nested"> Nested </RouterLink>
          </li>
        </ul>
        <div class="" d-flex>
          <button class="btn btn-outline-succes" type="" button @click="goPage">글 쓰기</button>
        </div>
      </div>
    </div>
  </nav>
</template>
