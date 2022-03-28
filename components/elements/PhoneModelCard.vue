<template>
  <div
    class="flex justify-between items-center border-gray-300 border rounded-xl hover:border-blue-500 cursor-pointer"
  >
    <div class="p-4">
      <h1>{{ this.modelName }}</h1>
      <p class="text-xs">{{ this.displaySize }} inch display<sup>1</sup></p>
    </div>
    <div class="p-4">
      <p>From {{ this.mmPrice }} Ks or <br />{{ this.tbPrice }} Baht</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ['modelName', 'displaySize', 'mmPrice', 'tbPrice'],
}
</script>
