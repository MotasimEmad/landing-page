<script setup>
const menu = ["Rankings", "Data", "Solution", "Pricing", "Resources"];
</script>

<template>
  <div :class="isDark ? 'dark' : ''" Class="bg-gray-100 dark:bg-gray-900">
    <div class="w-full min-h-screen font-sans bg-gray-100 dark:bg-gray-900">
      <div class="relative">
        <div class="relative py-10 px-8 mx-auto max-w-7xl">
          <nav class="flex flex-col md:flex-row justify-between items-center">
            <div>
              <a href="#" class="text-2xl font-semibold text-gray-900 dark:text-white">Liondo</a>
            </div>
            <div>
              <ul class="flex gap-6 tracking-wider text-gray-900 dark:text-gray-300">
                <li v-for="item in menu" v-bind:key="item.id">
                  <a href="#" class="transition hover:text-gray-600 dark:hover:text-white">
                    {{ item }}
                  </a>
                </li>
              </ul>
            </div>
            <div class="flex items-center">
              <button class="mt-4 md:mt-0 py-3 px-6 font-medium tracking-wider leading-5 text-gray-900 dark:text-white rounded-md border-2 border-gray-500 dark:border-gray-800 transition md:inline-block hover:bg-gray-900 hover:text-white dark:hover:bg-teal-300 dark:hover:text-gray-900 hover:shadow-lg">
                Get Started
              </button> 
              <button class="ml-2 mt-4 md:mt-0 py-2 px-6 font-medium tracking-wider leading-5 text-gray-900 dark:text-white rounded-md transition md:inline-block hover:bg-gray-900 hover:text-white dark:hover:bg-teal-300 dark:hover:text-gray-900 hover:shadow-lg" @click="isDark =! isDark">
                <svg v-if="isDark" class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 3v1m0 16v1m9-9h-1M4 12H3m15.364 6.364l-.707-.707M6.343 6.343l-.707-.707m12.728 0l-.707.707M6.343 17.657l-.707.707M16 12a4 4 0 11-8 0 4 4 0 018 0z"></path></svg>
                <svg v-else class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z"></path></svg>
              </button> 
            </div>
          </nav>
        </div>
      </div>
      <HeroComponent />
      <TrustComponent />
      <MarketComponent />
    </div>
  </div>
</template>

<style src="./assets/tailwind.css" />

<style>
    .toggle-checkbox:checked {
        right: 0;
        border: none;
        background-color: rgb(129 124 214);
        background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' className='h-10 w-10' fill='%23FFF' viewBox='0 0 24 24' stroke='rgb(129 124 214)' > <path strokeLinecap='round' strokeLinejoin='round' d='M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z' /> </svg>");
    }
    .toggle-checkbox:checked + .toggle-label {
        background-color: rgb(76 73 188);
    }   
</style>

<script>
import HeroComponent from './components/HeroComponent.vue'
import TrustComponent from './components/TrustComponent.vue'
import MarketComponent from './components/MarketComponent.vue'

export default {
  data() {
        return {
            isDark: false,
            isOpen: true,
        }
    },
  name: 'App',
  components: {
    HeroComponent,
    TrustComponent,
    MarketComponent
  }
}
</script>
