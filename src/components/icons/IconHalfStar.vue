<script setup lang="ts">
import { computed } from 'vue'

interface IconStarProps {
  small?: boolean
}
const props = withDefaults(defineProps<IconStarProps>(), {})

const width = computed(() => {
  return props.small ? '16' : '29'
})
</script>

<template>
  <svg
    :width="width"
    :height="width"
    stroke="currentColor"
    fill="currentColor"
    stroke-width="0"
    viewBox="0 0 576 512"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M288 0c-11.4 0-22.8 5.9-28.7 17.8L194 150.2 47.9 171.4c-26.2 3.8-36.7 36.1-17.7 54.6l105.7 103-25 145.5c-4.5 26.1 23 46 46.4 33.7L288 439.6V0z"
    ></path>
  </svg>
</template>
