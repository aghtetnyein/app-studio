<template>
  <div>
    <button
      v-if="variant === 'text'"
      :type="type"
      class="flex items-center gap-2"
      style="color: #0166cc"
    >
      <p class="text-md hover:underline">{{ label }}</p>
      <div><IconRightArrow /></div>
    </button>
    <button
      v-if="variant === 'contained'"
      :type="type"
      class="bg-blue-500 text-white rounded-full px-5 py-1 text-sm"
    >
      {{ label }}
    </button>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  props: ['type', 'variant', 'label'],
})
</script>
