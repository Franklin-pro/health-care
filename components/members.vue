<template>
  <div class="text-center  py-5">
      <h1 class="text-3xl font-semibold pb-3">Talk With Our Members</h1>
      <p class="">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur
        ducimus reprehenderit magni rerum dolor?
      </p>
    </div>
  <div class="grid lg:grid-cols-3 md:grid-cols-2 sm:grid-cols">
      <div v-for="item in items" :key="item.id" class="mx-auto mt-11 w-80 transform overflow-hidden rounded-lg bg-white dark:bg-slate-800 shadow-md duration-300 hover:scale-105 hover:shadow-lg"> 
  <div class="bg-red-100 w-[200px] ml-[50px] rounded-[50%]">
    <img
    class="h-48 w-full object-contain  object-center"
    src="../assets/doctor.png"
    alt="Product Image"
  />
  </div>

  <div class="p-4">
    <h2 class="mb-2 text-lg flex flex-col font-medium truncate text-[#10858c]">
      {{ item.title }}
    </h2>
    <h2>  {{ item.position }}</h2>
    <p class="mb-2 text-base dark:text-gray-300 text-gray-700">
    {{ item.description }}
    </p>
    <div class="flex items-center justify-between">
      <NuxtLink :to="`/products/`" class="text-md flex items-center gap-3 text-[#10858c]"><UIcon :name="item.icon"/></NuxtLink>
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
      title:"John Carter",
      icon:"i-heroicons-at-symbol",
      position:"CEO CO-FOUNDER",
      description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aspernatur ducimus hic autem sapiente nemo nesciunt iure laudantium ipsum!"
  },
  {
      id:2,
      title:"Sophie Moore",
      icon:"i-heroicons-bell-alert",
      position:"DENTAL SPECIALITY",
      description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aspernatur ducimus hic autem sapiente nemo nesciunt iure laudantium ipsum!"
  },
  {
      id:3,
      title:"Matt Cannon",
      icon:"i-heroicons-bell-alert",
      position:"ORTHOPEDIC",
      description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aspernatur ducimus hic autem sapiente nemo nesciunt iure laudantium ipsum!"
  },
  {
      id:3,
      title:"Andy Smith",
      icon:"i-heroicons-bell-alert",
      position:"BRAIN SURGEON",
      description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aspernatur ducimus hic autem sapiente nemo nesciunt iure laudantium ipsum!"
  },
  
]
</script>

<style>
/* Add your styles here */
</style>
