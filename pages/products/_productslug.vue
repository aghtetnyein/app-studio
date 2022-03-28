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
        <form id="phoneAddToBag" @submit.prevent="submitForm" method="post">
          <!-- phone model -->
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
              <div v-for="(phoneModel, index) in phoneModels" :key="index">
                <input
                  hidden
                  type="radio"
                  :id="phoneModel.name"
                  :value="phoneModel.name"
                  v-model="activePhoneModel"
                />
                <label :for="phoneModel.name">
                  <div
                    :class="`flex justify-between items-center border-gray-300 border rounded-xl xl:hover:border-blue-500 cursor-pointer ${
                      activePhoneModel === phoneModel.name && 'border-blue-500'
                    }`"
                  >
                    <div class="p-4">
                      <h1>{{ phoneModel.name }}</h1>
                      <p class="text-xs">
                        {{ phoneModel.displaySize }} inch display<sup>1</sup>
                      </p>
                    </div>
                    <div class="p-4">
                      <p>
                        From {{ phoneModel.mmPrice }} Ks or <br />{{
                          phoneModel.tbPrice
                        }}
                        Baht
                      </p>
                    </div>
                  </div>
                </label>
              </div>
            </div>
          </div>

          <div class="border-b border-gray-200 my-7"></div>

          <!-- phone color -->
          <div :class="`lg:px-6 ${activePhoneModel === '' && 'opacity-50'}`">
            <h1 class="mb-4 text-sm font-semibold">Choose your finish.</h1>
            <div class="grid grid-cols-2 gap-4">
              <div v-for="(color, index) in colors" :key="index">
                <input
                  hidden
                  :disabled="activePhoneModel === ''"
                  type="radio"
                  :id="color.name"
                  :value="color.name"
                  v-model="activeColor"
                />
                <label :for="color.name"
                  ><div
                    :class="`w-full text-center border-gray-300 border rounded-xl p-5 px-6
                    ${
                      activePhoneModel !== '' &&
                      'xl:hover:border-blue-500 cursor-pointer'
                    } 
                    ${activeColor === color.name && 'border-blue-500'}`"
                  >
                    <div
                      class="w-7 h-7 rounded-full mx-auto mb-2"
                      :style="`background-color: ${color.color}`"
                    ></div>
                    <span class="text-xs">{{ color.name }}</span>
                  </div></label
                >
              </div>
            </div>
          </div>
          <div class="border-b border-gray-200 my-7"></div>

          <!-- capacity -->
          <div :class="`lg:px-6 ${activeColor === '' && 'opacity-50'}`">
            <h1 class="my-4 text-sm font-semibold">Choose your capacity.</h1>
            <div class="grid grid-cols-2 gap-4">
              <div
                class="cursor-pointer"
                v-for="(capacity, index) in capacities"
                :key="index"
              >
                <input
                  hidden
                  :disabled="activeColor === ''"
                  type="radio"
                  :id="capacity.name"
                  :value="capacity.name"
                  v-model="activeCapacity"
                />
                <label :for="capacity.name"
                  ><div
                    :class="`w-full text-center border-gray-300 border rounded-xl p-2 py-4
                    ${
                      activeColor !== '' &&
                      'xl:hover:border-blue-500 cursor-pointer'
                    }
                    ${activeCapacity === capacity.name && 'border-blue-500'}`"
                  >
                    <h1 class="text-2xl mb-2 font-semibold">
                      {{ capacity.name }}<sup>2</sup>
                    </h1>
                    <p class="text-xs">
                      From {{ capacity.mmPrice }} Ks or <br />{{
                        capacity.tbPrice
                      }}
                      Baht
                    </p>
                  </div></label
                >
              </div>
            </div>
          </div>
          <div class="border-b border-gray-200 my-7"></div>

          <!-- currency -->
          <div :class="`lg:px-6 ${activeCapacity === '' && 'opacity-50'}`">
            <h1 class="my-4 text-sm font-semibold">Choose your currency.</h1>
            <div class="grid grid-cols-2 gap-4">
              <div
                class="cursor-pointer"
                v-for="(currency, index) in currencies"
                :key="index"
              >
                <input
                  hidden
                  :disabled="activeCapacity === ''"
                  type="radio"
                  :id="currency.name"
                  :value="currency.name"
                  v-model="activeCurrency"
                />
                <label :for="currency.name">
                  <div
                    :class="`text-center border-gray-300 border rounded-xl p-3 py-6
                    ${
                      activeCapacity !== '' &&
                      'xl:hover:border-blue-500 cursor-pointer'
                    }
                    ${activeCurrency === currency.name && 'border-blue-500'}`"
                  >
                    <h1 class="text-2xl font-semibold">{{ currency.name }}</h1>
                  </div>
                </label>
              </div>
            </div>
          </div>
          <div
            :class="`bg-gray-100 rounded-xl lg:mx-6 my-6 mb-0 p-6 ${
              activeCurrency === '' && 'opacity-50'
            }`"
          >
            <h1 class="text-2xl">3,400,000 Ks</h1>
            <button
              :disabled="activeCurrency === ''"
              type="submit"
              :class="`w-full bg-blue-500 py-2 rounded-lg text-white text-sm mt-4 ${
                activeCapacity === '' && 'cursor-default'
              }`"
            >
              Add to Bag
            </button>
            <p class="text-sm font-semibold mt-3">Still deciding?</p>
            <span class="text-sm"
              >Add this item to a list and easily come back to<br />
              it later.</span
            >
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'single-product',
  layout: 'products',

  data() {
    return {
      phoneModels: [
        {
          id: 1,
          name: 'iPhone 13 Pro',
          displaySize: '6.5',
          mmPrice: '3,100,000',
          tbPrice: '50,800',
        },
        {
          id: 2,
          name: 'iPhone 13 Pro Max',
          displaySize: '6.7',
          mmPrice: '3,100,000',
          tbPrice: '50,800',
        },
      ],
      colors: [
        {
          id: 1,
          name: 'Alpine green',
          color: '#496a4d',
        },
        {
          id: 2,
          name: 'Rose',
          color: '#ff0066',
        },
        {
          id: 3,
          name: 'Silver',
          color: '#c0c0c0',
        },
        {
          id: 4,
          name: 'Navy Blue',
          color: '#0066ff',
        },
      ],
      capacities: [
        {
          id: 1,
          name: '128GB',
          mmPrice: '3,100,000',
          tbPrice: '50,800',
        },
        {
          id: 2,
          name: '256GB',
          mmPrice: '3,400,000',
          tbPrice: '51,800',
        },
        {
          id: 3,
          name: '512GB',
          mmPrice: '3,100,000',
          tbPrice: '50,800',
        },
        {
          id: 4,
          name: '1TB',
          mmPrice: '3,400,000',
          tbPrice: '51,800',
        },
      ],
      currencies: [
        {
          id: 1,
          name: 'MMK',
        },
        {
          id: 2,
          name: 'TBH',
        },
      ],
      activePhoneModel: '',
      activeColor: '',
      activeCapacity: '',
      activeCurrency: '',
    }
  },

  methods: {
    submitForm() {
      let phoneAddToBagValues = {
        phoneModel: this.activePhoneModel,
        color: this.activeColor,
        capacity: this.activeCapacity,
        currency: this.activeCurrency,
      }
      console.log(phoneAddToBagValues)
      window.alert(JSON.stringify(phoneAddToBagValues))
    },
  },
})
</script>
