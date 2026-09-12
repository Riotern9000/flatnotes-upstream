<template>
  <div class="flex items-center">
    <svg
      width="36"
      height="36"
      viewBox="12 11 40 40"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
      class="text-theme-brand"
    >
      <path
        d="M32 16 C22 16 17 23 17 32 L17 46 C21 43 25 47 28 44 C30 42 34 42 36 44 C39 47 43 43 47 46 L47 32 C47 23 42 16 32 16 Z"
        fill="none"
        stroke="currentColor"
        stroke-width="3.5"
        stroke-linejoin="round"
        stroke-linecap="round"
      />
      <circle cx="26" cy="30" r="2.8" fill="currentColor" />
      <circle cx="38" cy="30" r="2.8" fill="currentColor" />
    </svg>
    <span
      class="ml-2.5 flex items-baseline font-bold tracking-tight text-xl"
      :class="{ 'hidden sm:inline-flex': props.responsive }"
    >
      <span class="text-theme-brand">Ghost</span>
      <span class="ml-1 text-theme-text font-medium">Notes</span>
    </span>
  </div>
</template>

<script setup>
const props = defineProps({
  responsive: {
    type: Boolean,
    default: false,
  },
});
</script>
