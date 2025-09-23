<script setup lang="ts">
import HeaderComponent from '@/components/HeaderComponent.vue';
import AboutComponent from '@/components/AboutComponent.vue';
import PhotosComponent from '@/components/PhotosComponent.vue';
import PresentComponent from '@/components/PresentComponent.vue';
import DetailsComponent from '@/components/DetailsComponent.vue';
import CreditComponent from '@/components/CreditComponent.vue';
import AddressComponent from '@/components/AddressComponent.vue';
import FooterComponent from '@/components/FooterComponent.vue';
</script>

<template>
  <div class="header-wrap">
    <HeaderComponent />
    <AboutComponent />
  </div>
  <PhotosComponent />
  <PresentComponent />
  <DetailsComponent />
  <CreditComponent />
  <AddressComponent />
  <FooterComponent />
</template>

<style lang="scss" scoped>
.header-wrap {
  padding: 0 30px 77px;
  background-image: url("../images/header-bg-mobile.jpg");

  @media(min-width: 1440px) {
    padding: 0 147px 159px;
    background-image: url("../images/header-bg-desktop.jpg");
  }
}
</style>
