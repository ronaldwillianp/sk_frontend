<script setup lang="ts">
import type { DropdownMenuItem } from '@nuxt/ui'

const items = ref<DropdownMenuItem[]>([
  {
    label: 'Profile',
    icon: 'i-lucide-user'
  },
  {
    label: 'Login',
    icon: 'i-lucide-cog'
  },
  {
    label: 'Logout',
    icon: 'i-lucide-credit-card'
  }

])
</script>

<template>
  <UDropdownMenu :items="items" :content="{
    align: 'start',
    side: 'bottom',
    sideOffset: 8
  }" :ui="{
    content: 'w-48'
  }">
    <UButton icon="i-lucide-user-round" color="neutral" variant="outline" />
  </UDropdownMenu>
</template>
