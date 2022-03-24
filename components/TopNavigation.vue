<template>
  <div class="">
    <div
      class="text-lg font-semibold bg-primary px-36 h-10 flex items-center justify-between"
    >
      <NuxtLink to="/">
        <AppLogo />
      </NuxtLink>

      <div class="flex gap-6">
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

      <div class="flex gap-6">
        <div class="cursor-pointer"><IconSearch /></div>
        <div class="cursor-pointer"><IconShoppingCart /></div>
        <div class="cursor-pointer"><IconAccount /></div>
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
})
</script>
