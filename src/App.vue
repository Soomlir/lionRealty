<script setup lang="ts">
import HeaderComponent from '@/components/HeaderComponent.vue';
import AboutComponent from '@/components/AboutComponent.vue';
import PhotosComponent from '@/components/PhotosComponent.vue';
</script>

<template>
  <div class="header-wrap">
    <HeaderComponent />
    <AboutComponent />
  </div>
  <PhotosComponent />
</template>

<style scoped>
.header-wrap {
  padding: 0 30px 77px;
  background-image: url("../images/header-bg-mobile.jpg");
}
</style>
