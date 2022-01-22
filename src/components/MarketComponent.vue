<script setup>
const features = [
  "Digital Marketing",
  "E-Commerce",
  "Digital Research",
  "Digital Analysis",
];
</script>

<template>
  <div class="py-16 px-14 mx-auto max-w-7xl">
    <div class="flex flex-col md:flex-row justify-between gap-x-6">
      <div class="md:w-1/2">
        <h2 class="text-2xl md:text-5xl font-bold leading-tight text-gray-800 dark:text-white">
          Must-Have to Win Your Online Market
        </h2>
      </div>
      <div class="w-1/2">
        <p class="pt-6 text-sm md:text-2xl leading-relaxed text-gray-500 dark:text-gray-300">
          Found something that works for you? Request a quote from our site or
          call an agent and we'll get back to you as soon as possible.
        </p>
        <button class="md:py-4 md:px-6 py-3 px-4 mt-4 font-medium tracking-wide rounded-lg transition bg-gray-900 dark:bg-teal-200 hover:bg-gray-700 dark:hover:bg-teal-300 text-white hover:text-white dark:text-black">
          Get Started
        </button>
      </div>
    </div>
    <div class="grid grid-cols-2 gap-4 items-center py-16 w-full md:grid-cols-4 md:gap-x-8">
      <div
        v-for="feature in features"
        v-bind:key="feature.id"
        class="group flex overflow-hidden relative flex-col items-start p-4 bg-gray-800 rounded-lg transition duration-300 cursor-pointer group dark:hover:bg-white"
      >
        <span
          class="inline-block font-medium tracking-wide text-white transition duration-300 group-dark:hover:text-gray-800"
        >
          {{ feature }}
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Market",
};
</script>
