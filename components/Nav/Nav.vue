<script lang="ts" setup>
const props = defineProps(['currentDay', 'opt1', 'opt1Link', 'opt2', 'opt2Link'])
</script>

<template>
  <div class="mb-10 flex w-full items-center justify-end bg-tertiary rounded">
    <div class="flex-1 pl-3 text-2xl md:text-3xl font-bold">
      {{ props.currentDay }}
    </div>
    <NuxtLink :to="opt1Link">
      <div class="bg-tertiary-500 px-6 md:px-8 py-2 md:py-4 text-2xl md:text-3xl font-bold">
        {{ props.opt1 }}
      </div>
    </NuxtLink>
    <NuxtLink :to="opt2Link">
      <div class="bg-tertiary-700 px-6 md:px-8 py-2 md:py-4 text-2xl md:text-3xl font-bold rounded-r">
        {{ props.opt2 }}
      </div>
    </NuxtLink>
  </div>
</template>
