<template>
  <div>
    <div
      class="fixed top-10 left-0 flex h-14 w-full mx-auto xl:px-32 justify-between items-center border-b border-gray-200 bg-white bg-opacity-80 z-10"
      style="backdrop-filter: blur(4px)"
    >
      <h1 class="font-semibold ml-10 text-lg">iPhone 13 Pro</h1>
    </div>

    <!-- end nav -->
    <div
      class="product-single grid md:grid-cols-2 md:gap-2 lg:gap-8 md:px-8 lg:px-24 xl:px-44 pt-0 pb-0"
    >
      <div
        class="w-full xl:w-4/5 h-full flex flex-col justify-center px-8 py-20 md:p-0"
      >
        <img
          src="/_mocks_/images/iPhone13Pro.png"
          alt="iphone13"
          class="w-60 h-80 mx-auto"
        />
        <div class="grid grid-cols-2 gap-4 items-start mt-16">
          <div class="flex flex-col gap-4 items-center">
            <IconDeliver />
            <p class="text-center text-xs font-semibold">
              Get free delivery, or pick up available Items at an App Studio
            </p>
          </div>
          <div class="flex flex-col gap-4 items-center">
            <IconReturn />
            <p class="text-center text-xs font-semibold">
              Free and easy return
            </p>
          </div>
        </div>
      </div>
      <div
        class="w-full xl:w-4/5 md:overflow-scroll scrollbar-hidden px-8 md:px-0 md:pt-20 pb-12"
      >
        <div class="lg:px-6">
          <div>
            <h1 class="text-red-500 font-thin text-xl">New</h1>
            <p class="text-4xl mt-2 font-semibold">Buy iPhone 13 Pro</p>
            <p class="text-sm text-gray-600 mt-2">
              Pre-order Now.Alpine Green available starting 3.18.
            </p>
            <p class="text-sm mt-4 font-semibold">Choose your model.</p>
          </div>
          <div class="mt-6 flex flex-col gap-4">
            <div
              class="flex justify-between items-center border-gray-300 border rounded-xl hover:border-blue-500 cursor-pointer"
            >
              <div class="p-4">
                <h1>iPhone 13 Pro</h1>
                <p class="text-xs">6.7 inch display<sup>1</sup></p>
              </div>
              <div class="p-4">
                <p>From 3,100,000 Ks or <br />50,800 Baht</p>
              </div>
            </div>
            <div
              class="flex justify-between items-center border-gray-300 border rounded-xl hover:border-blue-500 cursor-pointer"
            >
              <div class="p-4">
                <h1>iPhone 13 Pro</h1>
                <p class="text-xs">6.7 inch display<sup>1</sup></p>
              </div>
              <div class="p-4">
                <p>From 3,100,000 Ks or <br />50,800 Baht</p>
              </div>
            </div>
          </div>
        </div>
        <div class="border-b border-gray-200 my-7"></div>
        <div class="lg:px-6">
          <h1 class="mb-4 text-sm font-semibold">Choose your finish.</h1>
          <div class="grid grid-cols-2 gap-4">
            <div
              class="w-full text-center border-gray-300 border rounded-xl hover:border-blue-500 p-5 px-6 cursor-pointer"
            >
              <div
                class="w-7 h-7 rounded-full mx-auto mb-2"
                style="background-color: #496a4d"
              ></div>
              <span class="text-xs">Alpine green</span>
            </div>
            <div
              class="w-full text-center border-gray-300 border rounded-xl hover:border-blue-500 p-5 cursor-pointer"
            >
              <div class="w-7 h-7 bg-red-100 rounded-full mx-auto mb-2"></div>
              <span class="text-xs">Rose</span>
            </div>
            <div
              class="w-full text-center border-gray-300 border rounded-xl hover:border-blue-500 p-5 cursor-pointer"
            >
              <div class="w-7 h-7 bg-gray-200 rounded-full mx-auto mb-2"></div>
              <span class="text-xs">Silver</span>
            </div>
            <div
              class="w-full text-center border-gray-300 border rounded-xl hover:border-blue-500 p-5 cursor-pointer"
            >
              <div class="w-7 h-7 bg-blue-500 rounded-full mx-auto mb-2"></div>
              <span class="text-xs">Navy Blue</span>
            </div>
          </div>
        </div>
        <div class="border-b border-gray-200 my-7"></div>
        <div class="lg:px-6">
          <h1 class="my-4 text-sm font-semibold">Choose your capacity.</h1>
          <div class="grid grid-cols-2 gap-4">
            <div
              class="w-full text-center border-gray-300 border rounded-xl hover:border-blue-500 p-2 py-4 cursor-pointer"
            >
              <h1 class="text-2xl mb-2 font-semibold">128GB<sup>2</sup></h1>
              <p class="text-xs">From 3,100,000 Ks or <br />50,800 Baht</p>
            </div>
            <div
              class="w-full text-center border-gray-300 border rounded-xl hover:border-blue-500 p-2 py-4 cursor-pointer"
            >
              <h1 class="text-2xl mb-2 font-semibold">256GB<sup>2</sup></h1>
              <p class="text-xs">From 3,400,000 Ks or <br />51,800 Baht</p>
            </div>
            <div
              class="w-full text-center border-gray-300 border rounded-xl hover:border-blue-500 p-2 py-4 cursor-pointer"
            >
              <h1 class="text-2xl mb-2 font-semibold">512GB<sup>2</sup></h1>
              <p class="text-xs">From 3,100,000 Ks or <br />50,800 Baht</p>
            </div>
            <div
              class="w-full text-center border-gray-300 border rounded-xl hover:border-blue-500 p-2 py-4 cursor-pointer"
            >
              <h1 class="text-2xl mb-2 font-semibold">1TB<sup>2</sup></h1>
              <p class="text-xs">From 3,400,000 Ks or <br />51,800 Baht</p>
            </div>
          </div>
        </div>
        <div class="border-b border-gray-200 my-7"></div>
        <div class="lg:px-6">
          <h1 class="my-4 text-sm font-semibold">Choose your currency.</h1>
          <div class="grid grid-cols-2 gap-4">
            <div
              class="text-center border-gray-300 border rounded-xl hover:border-blue-500 p-3 py-6 cursor-pointer"
            >
              <h1 class="text-2xl mb-2 font-semibold">MMK</h1>
            </div>
            <div
              class="text-center border-gray-300 border rounded-xl hover:border-blue-500 p-3 py-6 cursor-pointer"
            >
              <h1 class="text-2xl mb-2 font-semibold">TBH</h1>
            </div>
          </div>
        </div>
        <div class="bg-gray-100 h-52 rounded-xl lg:mx-6 my-6 mb-0 p-6">
          <h1 class="text-2xl">3,400,000 Ks</h1>
          <button
            class="w-full bg-blue-500 py-2 rounded-lg text-white text-sm mt-4"
          >
            Add to Bag
          </button>
          <p class="text-sm font-semibold mt-3">Still deciding?</p>
          <span class="text-sm"
            >Add this item to a list and easily come back to<br />
            it later.</span
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'single-product',
  layout: 'products',
})
</script>
