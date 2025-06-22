<script setup lang="ts">
import SocialMediaCard from '@/components/SocialMediaCard.vue'
</script>

<template>
  <div class="main-wrapper h-full w-full flex justify-center items-center">
    <SocialMediaCard />
  </div>
</template>

<style scoped>
.main-wrapper {
  background: #020024;
  background: linear-gradient(
    90deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(9, 9, 121, 1) 35%,
    rgba(0, 212, 255, 1) 100%
  );
}
</style>
