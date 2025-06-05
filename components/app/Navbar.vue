<template>
  <header class="py-4 px-6 border-b  border-gray-200 shadow dark:border-gray-800">

    <div class="flex items-center justify-between">
      <div class="flex items-center flex-shrink-0  mr-6">
        <svg class="fill-current color-red-600 h-8 w-8 mr-2" width="54" height="54" viewBox="0 0 54 54"
          xmlns="http://www.w3.org/2000/svg">
          <path
            d="M13.5 22.1c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05zM0 38.3c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05z" />
        </svg>
        <span class="font-semibold text-xl tracking-tight">Tailwind CSS</span>
      </div>

      <div class="flex gap-6">
        <nav>
          <ul class="flex items-center gap-6">
            <li>
              <NuxtLink to="/" :activeClass="'text-red-500'">Home</NuxtLink>
            </li>
            <li>
              <NuxtLink to="/components" :activeClass="'text-red-500'">Components</NuxtLink>
            </li>
          </ul>
        </nav>

        <ColorModeButton />
        <DropdownMenuUser />
      </div>
    </div>
  </header>
</template>

<script lang="ts" setup>

</script>

<style scoped></style>