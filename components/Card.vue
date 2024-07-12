<template>
    <div class="grid lg:grid-cols-3 md:grid-cols-2 sm:grid-cols">
        <div v-for="item in items" :key="item.id" class="mx-auto mt-11 w-80 transform overflow-hidden rounded-lg bg-white dark:bg-slate-800 shadow-md duration-300 hover:scale-105 hover:shadow-lg"> 
    <img
      class="h-48 w-full object-contain object-center"
      src="../assets/doctor.png"
      alt="Product Image"
    />
    <div class="p-4">
      <h2 class="mb-2 text-lg font-medium truncate text-[#10858c]">
        {{ item.title }}
      </h2>
      <p class="mb-2 text-base dark:text-gray-300 text-gray-700 truncate">
      {{ item.description }}
      </p>
      <div class="flex items-center justify-between">
        <NuxtLink :to="`/products/`" class="text-md flex items-center gap-3 text-[#10858c]">Read More<UIcon name="i-heroicons-arrow-long-right"/></NuxtLink>
      </div>
    </div>
  </div>
    </div>
    
  <div
    class="grid lg:grid-cols-3 md:grid-cols-2 sm:grid-cols-1 gap-4 p-2 w-full"
  >
  
  </div>
</template>

<script lang="ts" setup>
  const items = [
    {
        id:1,
        title:"Dental treatments",
        description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aspernatur ducimus hic autem sapiente nemo nesciunt iure laudantium ipsum!"
    },
    {
        id:2,
        title:"Dental treatments",
        description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aspernatur ducimus hic autem sapiente nemo nesciunt iure laudantium ipsum!"
    },
    {
        id:3,
        title:"Dental treatments",
        description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aspernatur ducimus hic autem sapiente nemo nesciunt iure laudantium ipsum!"
    },
    {
        id:3,
        title:"Dental treatments",
        description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aspernatur ducimus hic autem sapiente nemo nesciunt iure laudantium ipsum!"
    },
    
  ]
  </script>

<style>
/* Add your styles here */
</style>
