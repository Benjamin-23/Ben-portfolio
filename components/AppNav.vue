<script lang="ts" setup>
const sideActive = ref(false)
const links = [ "Home", "About", 'Lab']
const newList: string[] = []
function activeMediaScreen(){
  sideActive.value = true
  for(let i of links){
    if (sideActive.value)
   newList.push(i)
   console.log(newList);
  }
}


</script>

<template>
  <div class="bg-blue-100">
  <div class="flex gap-1 justify-around items-center text-yellow-50 m-0 py-2">
    <img src="@/assets/images/Logo.svg" alt="logo" width="32">
    <div class="flex gap-16" v-if="sideActive" >

      <NuxtLink to="/" class=" hover:text-orange-400">Home</NuxtLink>
      <NuxtLink to="/#about" class="hover:text-orange-400">About</NuxtLink>
      <NuxtLink to="/lab" class="hover:text-orange-400" >Lab</NuxtLink>
    </div>
    <div class="" v-else> 
      <button class="text-white " @click="activeMediaScreen()">Menu
      </button>
     
    </div>

  </div>
  </div>
</template>