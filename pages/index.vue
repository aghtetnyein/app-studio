<template>
  <div>
    <p class="font-bold">HEllO</p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'home',
  layout: 'main',

  head() {
    return {
      title: 'Home - App Studio',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Mobile Phone Ecoomerce Site',
        },
        {
          hid: 'keywords',
          name: 'keywords',
          content: 'appstudio, ecommerece, mobilephone, mobile, phone,',
        },
      ],
    }
  },
})
</script>
