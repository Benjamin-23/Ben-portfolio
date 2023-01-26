<script lang="ts" setup>
const sideActive = ref(false)
function activeMediaScreen() {
  // sideActive.value = true
  sideActive.value = !sideActive.value

}


</script>

<template>
  <div class="bg-blue-100  max-md:hidden">
    <div class="flex gap-1 justify-around items-center text-yellow-50 m-0 py-2">
      <img src="@/assets/images/Logo.svg" alt="logo" width="32">
      <div class="flex gap-16">
        <NuxtLink to="/" class=" hover:text-orange-400">Home</NuxtLink>
        <NuxtLink to="/#about" class="hover:text-orange-400">About</NuxtLink>
        <NuxtLink to="#lab" class="hover:text-orange-400">Lab</NuxtLink>
      </div>

    </div>
  </div>
  <div class="md:hidden">
    <Transition name="slide-fade">
      <div class="flex flex-col md:hidden text-white bg-blue-300 gap-1 px-2 fixed top-0 w-full py-1 z-10"
        v-if="sideActive">
        <p class=" text-right text-xl" @click="activeMediaScreen()">X</p>
        <div class="flex flex-col text-[17px] gap-1 ">
          <a class="hover:text-orange-400" href="/" @click="activeMediaScreen()"> Home</a>
          <a  class="hover:text-orange-400" href="#about" @click="activeMediaScreen()">About </a>
          <a  class="hover:text-orange-400 bg-none"  href="#lab" @click="activeMediaScreen()">Lab</a>
        </div>

      </div>
      <div class="flex w-full bg-blue-100 justify-around items-center py-2 fixed top-0 " v-else>
        <img src="@/assets/images/Logo.svg" alt="logo" width="32">
        <button class="text-white md:hidden" @click="activeMediaScreen()"><img src="@/assets/images/Humberger.svg"
            alt="" class="w-10">
        </button>
      </div>
    </Transition>
  </div>
</template>
<style>
.slide-fade-enter-active {
  transition: all 0.3s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.4s;
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateX(-20px);
  opacity: 0;
}
</style>