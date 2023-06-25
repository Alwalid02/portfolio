<template>
    <!-- <div class="card text-center">
      <img :src="`${product.image}`" class="thumb" />
      <p class="font-bold text-gray-500 m-4 truncate">{{ product.title }}</p>
      <NuxtLink :to="`/products/${product.id}`">
        <p class="btn my-4">View Details</p>
      </NuxtLink>
    </div> -->
    
<div class="max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700">
    <NuxtLink :to="`/products/${product.id}`">
        <img class="thumb" :src="`${product.image}`" alt="" />
    </NuxtLink>
    <div class="p-5">
        <NuxtLink :to="`/products/${product.id}`">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">{{ product.title }}</h5>
        </NuxtLink>
        <!-- <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.</p> -->
        <NuxtLink :to="`/products/${product.id}`" class="inline-flex items-center px-3 py-2 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
            Read more
            <svg aria-hidden="true" class="w-4 h-4 ml-2 -mr-1" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
        </NuxtLink>
    </div>
</div>

  </template>
  
  <script setup>
    const { product } = defineProps(['product'])
  </script>
  
  <style scoped>
    .thumb {
      max-height: 120px;
      max-width: 70%;
      margin: 0 auto;
    }
  </style>