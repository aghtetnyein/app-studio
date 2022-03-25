<template>
  <div>
    <div
      class="bg-white w-screen flex gap-2 md:justify-center p-2 overflow-x-scroll scrollbar-hidden"
    >
      <div class="cursor-pointer hover:bg-gray-100 p-4 rounded-md">
        <SvgShopIphone />
        <div class="mt-3 text-center">
          <p class="text-xs">Shop iPhone</p>
          <!-- <p class="text-xs text-red-500">New</p> -->
        </div>
      </div>
      <div class="cursor-pointer hover:bg-gray-100 p-4 rounded-md">
        <SvgIphone13Pro />
        <div class="mt-3 text-center">
          <p class="text-xs">iPhone 13 Pro</p>
          <p class="text-xs text-red-500">New</p>
        </div>
      </div>
      <div class="cursor-pointer hover:bg-gray-100 p-4 rounded-md">
        <SvgIphone13 />
        <div class="mt-3 text-center">
          <p class="text-xs">iPhone 13</p>
          <p class="text-xs text-red-500">New</p>
        </div>
      </div>
      <div class="cursor-pointer hover:bg-gray-100 p-4 rounded-md">
        <SvgIphoneSE />
        <div class="mt-3 text-center">
          <p class="text-xs">iPhone SE</p>
          <p class="text-xs text-red-500">New</p>
        </div>
      </div>
      <div class="cursor-pointer hover:bg-gray-100 p-4 rounded-md">
        <SvgIphone12 />
        <div class="mt-3 text-center">
          <p class="text-xs">iPhone 12</p>
          <!-- <p class="text-xs text-red-500">New</p> -->
        </div>
      </div>
      <div class="cursor-pointer hover:bg-gray-100 p-4 rounded-md">
        <SvgIphone11 />
        <div class="mt-3 text-center">
          <p class="text-xs">iPhone 11</p>
          <!-- <p class="text-xs text-red-500">New</p> -->
        </div>
      </div>
    </div>

    <div class="flex flex-col items-center py-12">
      <h2 class="text-4xl text-gray-800 font-medium">Shop iPhone</h2>
      <p class="mt-4 text-xl text-gray-700 font-normal">
        All models. <span class="text-gray-400">Take your pick.</span>
      </p>

      <div
        class="my-12 w-full px-8 md:px-16 lg:px-10 xl:px-56 grid md:grid-cols-2 lg:grid-cols-3 gap-6"
      >
        <ElementProductCard />
        <ElementProductCard />
        <ElementProductCard />
        <ElementProductCard />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'products',
  layout: 'main',
})
</script>
