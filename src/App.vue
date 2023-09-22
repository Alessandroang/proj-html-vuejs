<script setup>
import AppFooter from "./components/AppFooter.vue";
import AppHeader from "./components/AppHeader.vue";
import Slider from "./components/Content/Slider.vue";
import TrainingBox from "./components/Content/TrainingBox.vue";
import BikeEvents from "./components/Content/BikeEvents.vue";
import OurBiker from "./components/Content/OurBiker.vue";
import ResentArticles from "./components/Content/ResentArticles.vue";
import SpecialPacks from "./components/Content/SpecialPacks.vue";
import Loader from "./components/Content/Loader.vue";
</script>

<template>
  <Loader />
  <AppHeader />
  <Slider />
  <TrainingBox />
  <BikeEvents />
  <OurBiker />
  <SpecialPacks />
  <ResentArticles />
  <AppFooter />
</template>

<style></style>
