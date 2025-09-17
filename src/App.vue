<script setup lang="ts">
import HeaderComponent from '@/components/HeaderComponent.vue';
import AboutComponent from '@/components/AboutComponent.vue';
</script>

<template>
  <div class="header-wrap">
    <HeaderComponent />
    <AboutComponent />
  </div>
</template>

<style scoped>
.header-wrap {
  background-image: url("../images/header-bg-mobile.jpg");
}
</style>
