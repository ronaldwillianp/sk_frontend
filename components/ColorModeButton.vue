<template>
  <ClientOnly v-if="!colorMode?.forced">
    <UButton class="border-1" :icon="isDark ? 'i-lucide-moon' : 'i-lucide-sun'" color="neutral" variant="ghost"
      @click="isDark = !isDark" />

    <template #fallback>
      <div class="size-8" />
    </template>
  </ClientOnly>
</template>

<script setup>
const colorMode = useColorMode()

const isDark = computed({
  get() {
    return colorMode.value === 'dark'
  },
  set(_isDark) {
    colorMode.preference = _isDark ? 'dark' : 'light'
  }
})
</script>

