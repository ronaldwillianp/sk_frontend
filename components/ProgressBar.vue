<template>
  <div class="max-w-80">
    <UProgress v-model="estado" :max="['Waiting...', 'Cloning...', 'Migrating...', 'Deploying...', 'Done!']" />
  </div>
</template>

<script setup lang="ts">
const estado = ref(0)
const clock = () => {
  if (estado.value == 4) {
    estado.value = 0
  } else {
    estado.value += 1
  }
}

onNuxtReady(async () => {
  setInterval(clock, 2000)
})

</script>

<style></style>