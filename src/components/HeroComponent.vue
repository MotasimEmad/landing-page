<template>
  <div class="relative py-6 px-8 max-w-7xl">
    <div class="flex flex-col lg:flex-row text-start">
        <div class="lg:w-1/2">
          <h1 class="text-2xl md:text-5xl lg:text-7xl font-bold leading-tight text-gray-800 dark:text-white">
            Tracking User
            <span class="relative after:bottom-2 after:left-0 after:bg-gradient-to-l after:from-teal-300 after:absolute after:w-80 after:h-5 after:-z-10">
              Movements
            </span>
            Around the World
          </h1>
            <p class="pt-2 max-w-lg text-sm md:text-2xl tracking-wide leading-relaxed text-gray-500 dark:text-gray-300">
              Whether it's your family or your business, we want to help you take
              care of the things that matter the most.
            </p>

            <div class="flex gap-x-6 items-center pt-12">
              <button class="md:py-4 md:px-6 py-3 px-4 font-medium tracking-wide bg-gray-900 dark:bg-teal-200 hover:bg-gray-700 dark:hover:bg-teal-300 text-white hover:text-white dark:text-black rounded-lg shadow-md transition">
                Get Trial Project
              </button>
              <button class="md:py-4 md:px-6 flex gap-x-2 items-center py-3 px-4 font-medium tracking-wide text-gray-900 dark:text-gray-300 transition hover:text-gray-700 dark:hover:text-teal-300">
                <svg class="w-8 h-8 stroke-current" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.2" d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z"></path>
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.2" d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                </svg>
                <span>Watch Demo</span>
              </button>
            </div>
        </div>
         <div class="flex items-center md:justify-center lg:w-1/2">
          <img
            class="md:mt-28 lg:mt-12 lg:max-w-xl drop-shadow-2xl md:animate-bounce"
            :src="'/img/hero.png'"
            alt=""
          />
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Hero'
}
</script>
