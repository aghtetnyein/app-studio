<template>
  <div>
    <div class="fixed w-screen z-30">
      <div
        class="text-lg font-semibold bg-primary px-4 md:px-10 xl:px-36 flex items-center justify-between h-10"
      >
        <div class="flex gap-4">
          <NuxtLink to="/">
            <AppLogo />
          </NuxtLink>
        </div>

        <div class="hidden lg:flex gap-6">
          <div
            class="cursor-pointer"
            v-for="(category, index) in categories"
            :key="index"
          >
            <p class="text-sm text-gray-400 font-normal hover:text-white">
              {{ category.name }}
            </p>
          </div>
        </div>

        <div class="flex items-center gap-4 lg:gap-6">
          <div class="flex lg:hidden items-center relative">
            <input
              class="py-1 px-2 rounded-md w-full border border-gray-500 focus:outline-none focus:border-gray-400 focus:ring-0.5 focus:ring-gray-400 text-sm text-black"
              type="text"
              placeholder="Search"
            />
            <!-- <div class="absolute right-2 text-gray-400">
              <IconSearch />
            </div> -->
          </div>
          <div class="hidden lg:block cursor-pointer text-gray-200">
            <IconSearch />
          </div>
          <div class="cursor-pointer text-gray-200"><IconShoppingCart /></div>
          <div class="hidden lg:block cursor-pointer text-gray-200">
            <IconAccount />
          </div>

          <div class="lg:hidden">
            <button
              class="text-white w-5 h-10 relative focus:outline-none"
              @click="toggleMobileNav()"
              @blur="closeMobileNav()"
            >
              <span class="sr-only">Open main menu</span>
              <div
                class="block w-5 absolute left-1/2 top-1/2 transform -translate-x-1/2 -translate-y-1/2"
              >
                <span
                  aria-hidden="true"
                  class="block absolute h-0.5 w-5 bg-current transform transition duration-500 ease-in-out"
                  :class="{
                    'rotate-45': mobileNavOpen,
                    ' -translate-y-1.5': !mobileNavOpen,
                  }"
                ></span>
                <span
                  aria-hidden="true"
                  class="block absolute h-0.5 w-5 bg-current transform transition duration-500 ease-in-out"
                  :class="{ 'opacity-0': mobileNavOpen }"
                ></span>
                <span
                  aria-hidden="true"
                  class="block absolute h-0.5 w-5 bg-current transform transition duration-500 ease-in-out"
                  :class="{
                    '-rotate-45': mobileNavOpen,
                    ' translate-y-1.5': !mobileNavOpen,
                  }"
                ></span>
              </div>
            </button>
          </div>
        </div>
      </div>
    </div>

    <div
      :class="`fixed top-0 left-0 z-20 bg-primary transition-all ease-in-out duration-300 w-screen overflow-hidden  ${
        mobileNavOpen ? 'h-screen' : 'h-0'
      }`"
    >
      <div class="mt-10">
        <div class="border-b border-gray-500 my-6"></div>

        <div class="px-6 md:px-24">
          <div
            class="cursor-pointer py-2"
            v-for="(category, index) in categories"
            :key="index"
          >
            <p class="text-sm text-gray-300 font-normal hover:text-white">
              {{ category.name }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'top-navigation',

  data() {
    return {
      mobileNavOpen: false,
      categories: [
        {
          name: 'Mac',
          slug: 'mac',
          icon: '💻',
        },
        {
          name: 'iPad',
          url: 'i-pad',
          icon: '📱',
        },
        {
          name: 'iPhone',
          url: 'i-phone',
          icon: '📱',
        },
        {
          name: 'Watch',
          url: 'watch',
          icon: '⌚',
        },
        {
          name: 'AirPods',
          url: 'air-pods',
          icon: '🎧',
        },
        {
          name: 'TV & Home',
          url: 'tv-home',
          icon: '📺',
        },
        {
          name: 'Only on Apple',
          url: 'only-apple',
          icon: '🍎',
        },
        {
          name: 'Accessories',
          url: 'accessories',
          icon: '🎁',
        },
        {
          name: 'Support',
          url: 'support',
          icon: '💁',
        },
      ],
    }
  },

  methods: {
    toggleMobileNav() {
      this.mobileNavOpen = !this.mobileNavOpen
    },
    closeMobileNav() {
      this.mobileNavOpen = false
    },
  },
})
</script>
