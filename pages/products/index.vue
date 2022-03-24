<template>
  <div>
    <p class="font-bold">This is all products</p>
    <ElementProductCard />
  </div>
</template>

//
<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'products',
  layout: 'main',
})
</script>
