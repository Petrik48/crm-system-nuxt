<script lang="ts" setup>
  const props = defineProps({
    labelText: {
      type: String,
      default: '',
    },
  })
</script>

<template>
  <div class="mb-3">
    <label v-if="labelText" class="opacity-75 mb-0.5 block text-xs">
      {{ labelText }}
    </label>
    <div class="text-base">
      <slot></slot>
    </div>
  </div>
</template>