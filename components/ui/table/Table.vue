<script setup lang="ts">
import type { HTMLAttributes } from 'vue'
import { cn } from '@/lib/utils'

const props = defineProps<{
  class?: HTMLAttributes['class']
}>()
</script>

<template>
  <div class="relative w-full overflow-x-auto overflow-y-hidden">
    <table :class="cn('w-full border-collapse border-spacing-0 caption-bottom text-sm', props.class)">
      <slot />
    </table>
  </div>
</template>
