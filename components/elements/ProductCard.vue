<template>
  <div class="bg-white rounded-lg shadow-md px-4 py-5">
    <div class="p-4">
      <p class="uppercase text-xs text-blue-500">
        <span class="text-red-500">New</span> Available - 2 - Alpine Green
      </p>
      <h5 class="font-bold text-md mt-1">iPhone 13 Pro</h5>
    </div>
    <div class="mx-auto my-3 flex justify-center">
      <img
        class="w-32 h-44"
        src="/_mocks_/images/iPhone13Pro.png"
        alt="Mountain"
      />
    </div>
    <div class="flex justify-center my-6 gap-1">
      <div class="w-3 h-3 bg-green-300 rounded-full"></div>
      <div class="w-3 h-3 bg-purple-200 rounded-full"></div>
      <div class="w-3 h-3 bg-red-100 rounded-full"></div>
      <div class="w-3 h-3 bg-gray-400 rounded-full"></div>
      <div class="w-3 h-3 bg-blue-200 rounded-full"></div>
    </div>
    <div class="mt-6 flex items-center justify-between">
      <div>
        <p class="text-xs">Price 2,300,000 Ks or</p>
        <p class="mt-1 text-xs">42,600 Baht.</p>
      </div>
      <NuxtLink to="/products/iphone-13-pro"
        ><ElementButton type="button" variant="contained" label="Pre-order"
      /></NuxtLink>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'product-card',
})
</script>
