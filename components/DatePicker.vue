<template>
  <div class="max-w-80">
    <UCalendar :default-value="defaultValue" />
  </div>
</template>

<script setup lang="ts">
import { CalendarDate, startOfWeek } from '@internationalized/date';
const defaultValue = ref(new CalendarDate(2025, 2, 6))
</script>

<style>

</style>