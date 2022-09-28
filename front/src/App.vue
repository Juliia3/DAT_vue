<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/Header/Header.vue';
// import Search from './components/Search/Search.vue';
import './assets/styles/index.scss'

</script>

<template>
    <div class="page-wrapper">
      <Header /> 
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>

  <RouterView />
</template>
