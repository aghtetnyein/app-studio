<template>
  <div>
    <div class="h-10 bg-gray-200 flex items-center justify-center gap-4">
      <img src="/MobileWorldLogo.png" class="h-6" alt="mobile-world-logo" />
      <p class="text-xs">
        Website မှ ကြိုက်နှစ်သက်ရာ မည်သည့်ပစ္စည်းကိုမဆို ဝယ်ယူအားပေးမှုအတွက် ၄၈
        နာရီအတွင်း အိမ်တိုင်ရာရောက် အခမဲ့ဝန်ဆောင်မှုဖြင့် ဆောင်ရွက်ပေးနေပါသည်။
      </p>
    </div>

    <div class="py-20">
      <div class="flex flex-col items-center text-center">
        <h2 class="text-5xl text-gray-800 font-medium">iPhone 13 Pro</h2>
        <p class="mt-4 text-2xl text-gray-700 font-normal">
          Now in Alpine Green.
        </p>
        <p class="mt-3 text-xl text-gray-400 font-normal">
          Available starting 3.18
        </p>
        <div class="mt-3 flex items-center justify-center gap-12">
          <ElementButton type="button" variant="text" label="Learn more" />
          <ElementButton type="button" variant="text" label="Shop" />
        </div>
      </div>
      <div class="mt-4 w-full flex justify-center">
        <img
          src="/_mocks_/images/iPhone13ProLanding.png"
          class="h-96"
          alt="iPhone13Pro"
        />
      </div>
    </div>

    <div class="py-16">
      <div class="flex flex-col items-center text-center">
        <p class="mt-3 text-xl text-gray-800 font-semibold">The new</p>
        <img src="/_mocks_/images/iPhoneSETitle.png" alt="" class="h-14" />
        <p class="mt-4 text-2xl text-gray-700 font-normal">
          Love the power. Love the price.
        </p>
        <p class="mt-3 text-xl text-gray-400 font-normal">
          Available starting 3.18
        </p>
        <div class="mt-3 flex items-center justify-center gap-12">
          <ElementButton type="button" variant="text" label="Learn more" />
          <ElementButton type="button" variant="text" label="Pre-order" />
        </div>
      </div>
      <div class="mt-4 w-full flex justify-center">
        <img src="/_mocks_/images/iPhoneSE.png" class="h-80" alt="iPhoneSE" />
      </div>
    </div>

    <div class="bg-black py-12 px-52 flex gap-8 items-center justify-center">
      <div class="w-full flex flex-col items-center text-center">
        <img src="/_mocks_/images/iPadAirTitle.png" alt="" class="h-14" />
        <p class="mt-4 text-2xl text-gray-100 font-normal">
          Light. Bright. Full of might.
        </p>
        <p class="mt-3 text-xl text-gray-500 font-normal">
          Available starting 3.18
        </p>
        <div class="mt-3 flex items-center justify-center gap-12">
          <ElementButton type="button" variant="text" label="Learn more" />
          <ElementButton type="button" variant="text" label="Order now" />
        </div>
      </div>
      <div class="flex justify-center">
        <img
          src="/_mocks_/images/iPadAir.png"
          class="w-full h-full"
          alt="iPadAir"
        />
      </div>
    </div>

    <div class="grid grid-cols-2 p-6 gap-6">
      <!-- StudioDisplay -->
      <div class="bg-gray-100 py-8 rounded-lg flex flex-col justify-between">
        <div class="w-full flex flex-col items-center text-center">
          <h2 class="text-4xl text-gray-800 font-medium">Studio Display</h2>
          <p class="mt-2 text-xl text-gray-700 font-normal">
            A sight to be bold.
          </p>
          <p class="mt-1 text-xl text-gray-400 font-normal">
            Available starting 3.18
          </p>
          <div class="mt-2 flex items-center justify-center gap-12">
            <ElementButton type="button" variant="text" label="Learn more" />
            <ElementButton type="button" variant="text" label="Order now" />
          </div>
        </div>
        <div class="mt-8 flex justify-center">
          <img
            src="/_mocks_/images/StudioDisplay.png"
            class="h-72"
            alt="StudioDisplay"
          />
        </div>
      </div>

      <!-- Mac Studio -->
      <div class="bg-gray-100 py-8 rounded-lg flex flex-col justify-between">
        <div class="w-full flex flex-col items-center text-center">
          <h2 class="text-4xl text-gray-800 font-medium">Mac Studio</h2>
          <p class="mt-2 text-xl text-gray-700 font-normal">Empower station.</p>
          <p class="mt-1 text-xl text-gray-400 font-normal">
            Available starting 3.18
          </p>
          <div class="mt-2 flex items-center justify-center gap-12">
            <ElementButton type="button" variant="text" label="Learn more" />
            <ElementButton type="button" variant="text" label="Order now" />
          </div>
        </div>
        <div class="mt-8 flex justify-center">
          <img
            src="/_mocks_/images/MacStudio.png"
            class="h-52"
            alt="MacStudio"
          />
        </div>
      </div>

      <!-- iPhone 13 -->
      <div class="bg-gray-100 pt-8 rounded-lg flex flex-col justify-between">
        <div class="w-full flex flex-col items-center text-center">
          <h2 class="text-4xl text-gray-800 font-medium">iPhone 13</h2>
          <p class="mt-2 text-xl text-gray-700 font-normal">Now in Green.</p>
          <p class="mt-1 text-xl text-gray-400 font-normal">
            Available starting 3.18
          </p>
          <div class="mt-2 flex items-center justify-center gap-12">
            <ElementButton type="button" variant="text" label="Learn more" />
            <ElementButton type="button" variant="text" label="Shop" />
          </div>
        </div>
        <div class="mt-8 flex justify-center">
          <img
            src="/_mocks_/images/iPhone13ProductLanding.png"
            class="h-60"
            alt="iPhone13"
          />
        </div>
      </div>

      <!-- Watch -->
      <div class="bg-gray-100 py-8 rounded-lg flex flex-col justify-between">
        <div class="w-full flex flex-col items-center text-center">
          <img
            src="/_mocks_/images/watchTitle.png"
            class="h-14"
            alt="iPhone13"
          />
          <p class="mt-2 text-xl text-gray-400 font-normal">
            It's our largest display yet.
          </p>
          <div class="mt-2 flex items-center justify-center gap-12">
            <ElementButton type="button" variant="text" label="Learn more" />
            <ElementButton type="button" variant="text" label="Buy" />
          </div>
        </div>
        <div class="mt-8 flex justify-center">
          <img src="/_mocks_/images/Watch.png" class="h-60" alt="Watch" />
        </div>
      </div>

      <!-- Card -->
      <div
        class="col-span-2 bg-gray-100 py-8 rounded-lg flex flex-col justify-between"
      >
        <div class="w-full flex flex-col items-center text-center">
          <img src="/_mocks_/images/cardTitle.png" class="h-8" alt="iPhone13" />
          <p class="mt-4 text-xl text-gray-700 font-normal w-64">
            Get up to 3% daily cash back with every purchase.
          </p>
          <div class="mt-2 flex items-center justify-center gap-12">
            <ElementButton type="button" variant="text" label="Learn more" />
            <ElementButton type="button" variant="text" label="Shop" />
          </div>
        </div>
        <div class="mt-8 flex justify-center">
          <img src="/_mocks_/images/Card.png" class="h-80" alt="Card" />
        </div>
      </div>
    </div>
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
