<template>
    <div class="p-8">
<div class="grid lg:grid-cols-2 gap-6 items-center justify-between pb-4">
    <div>
<h1 class="text-3xl pb-6">Providing Quality <span class="text-[#1cacb4]">Healthcare</span> for a <span class="text-[#88ba5c]">Brighter </span>and <span class="text-[#88ba5c]">Healthy</span> Future</h1>
<p class="text-xl">At our hospital, we are dedicated to providing exceptional
     medical care to our patients and their families. 
     Our experienced team of medical professionals,
      cutting-edge technology, and compassionate approach 
      make us a leader in the healthcare industry</p>
      
      <div class="flex gap-6 items-center justify-center py-6">
        <Button>Appointments</Button>
        <div class="bg-[#10858c] text-white cursor-pointer inline p-2 rounded-[50%] flex items-center">
            <UIcon name="i-heroicons-play" solid/>
        </div>
        <h1>Watch Video</h1>
        
      </div>
    
    </div>
    <div class="bg-gradient-to-t from-[#88ba5c] to-[#1cacb4]  rounded-[100%] rounded-r-[80%]">
        <img src="../assets/doctor.png" alt="">
    </div>
   
</div>
<div class="bg-gray-100 rounded-xl flex items-center justify-between p-4">
    <div class="">
        <h1 class="pb-4 font-bold">Find The Doctor</h1>
        <div class="flex gap-5">
            <UInput type="text" placeholder="Name"/>
            <UInput type="text" placeholder="Speciality"/>
        </div>
       
    </div>
   <div class="flex gap-5 items-center">
    <h1>Avialable <UToggle v-model="selected"></UToggle></h1>
    <Button>Search</Button>
   </div>
</div>
    </div>
    <About/>
    <Services/>
    <Members/>
</template>

<script setup>
const selected= ref(true)
</script>

<style scoped>

</style>