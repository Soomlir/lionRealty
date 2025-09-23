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
  <div class="app-wrap">
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
  </div>
</template>

<style lang="scss" scoped>
.app-wrap {
  width: 320px;
  margin: 0 auto;

  @media (min-width: 1440px) {
    width: 1440px;
  }
}

.header-wrap {
  padding: 0 30px 77px;
  background-image: url("../images/header-bg-mobile.jpg");

  @media(min-width: 1440px) {
    padding: 0 147px 159px;
    background-image: url("../images/header-bg-desktop.jpg");
  }
}
</style>
