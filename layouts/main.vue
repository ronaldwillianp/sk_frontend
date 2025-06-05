<template>
  <div>
    <Navbar />
    <slot />
    <Footer />
  </div>
</template>

<script lang="ts" setup>
import Navbar from '~/components/app/Navbar.vue';
import Footer from '~/components/app/Footer.vue';
</script>

<style scoped></style>