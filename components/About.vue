<template>
  <UContainer>
    <div class="p-8">
    <h1 class="text-center text-2xl font-semibold">Our Result in Number</h1>
    <div class="flex justify-between">
      <div v-for="item in items" :key="item.id">
        <h1 class="font-bold py-4 text-3xl text-center text-[#10858c]">
          {{ item.number }}
        </h1>
        <h1 class="font-semibold">{{ item.title }}</h1>
      </div>
    </div>
    <div class="flex pt-8 justify-around items-center">
      <div class="w-[50%]">
        <h1 class="text-2xl text-[#10858c] pb-3 font-semibold">You have lots of reasons to choose us</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste
          perspiciatis excepturi iusto, voluptatem alias quos.
        </p>
        <div class="flex py-5 gap-6">
          <Button>Get Started</Button>
          <UButton class="bg-gray-500">Talk to Sale</UButton>
          <!-- <Button>talk to Sale</Button> -->
        </div>
      </div>
      <div class="w-[300px]">
        <img src="../assets/doctor.png" alt="" />
      </div>
    </div>
  </div>
  </UContainer>
 
</template>

<script lang="ts" setup>
const items = [
  {
    id: 1,
    number: "90%",
    title: "Customers Satisfaction",
  },
  {
    id: 2,
    number: "15k",
    title: "Online Patients",
  },
  {
    id: 3,
    number: "12k",
    title: "Patients Recovered",
  },
  {
    id: 4,
    number: "240%",
    title: "Campany Growth",
  },
];
</script>

<style></style>
