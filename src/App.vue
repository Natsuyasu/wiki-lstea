<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup

import GlobalFooter from './components/GlobalFooter.vue';
import HomeHeader from './components/HomeHeader.vue';
import SideBar from './components/SideBar.vue';
</script>

<template>
  <HomeHeader />
  <SideBar />
  <div class="container mx-auto my-5">
    <div class="flex sm:justify-center space-x-4" id="nav">
      <router-link
        to="/"
        class="rounded-lg px-3 py-2 text-slate-700 font-medium hover:bg-slate-100 hover:text-slate-900"
        >Home</router-link
      >
      <router-link
        to="/about"
        class="rounded-lg px-3 py-2 text-slate-700 font-medium hover:bg-slate-100 hover:text-slate-900"
        >About</router-link
      >
    </div>
    <router-view />
  </div>
  <GlobalFooter />
</template>
