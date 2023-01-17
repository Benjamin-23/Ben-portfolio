<script lang="ts" setup>
const runtimeConfig = useRuntimeConfig()
const appConfig = useAppConfig()
</script>
<template>
  <NuxtLayout>
    <div class="flex mt-12 w-full justify-center">
      <div class="flex flex-col max-w-[60%] gap-4 max-md:max-w-[80%]">
        <!-- Homre page -->
        <!--  -->
        <div class="flex flex-col w-full gap-6">
          <div class="flex">
            <div class="radical-bg justify-center items-center flex">
              <img src="@/assets/images/profile.svg" alt="loading" class="w-60">
            </div>
            <div class="flex-col relative gap-10 flex ml-[-20px] text-white mt-4 max-sm:gap-6 max-sm:mt-3">
              <div class="flex w-full gap-6 justify-evenly">
                <p class=" w-full text-m">Hello! I Am <span class=" text-blue-200">Basilica Benjamin</span></p>
              </div>
              <div class="flex flex-col gap-2">
                <p class="font-[Preahvihear, poppins] text-sm underline">A Designer who</p>
                <h1 class="font-bold text-[2em] max-sm:text-[1.5em]">Judges a book <br> by its <span
                    class="text-blue-200 cover p-1 ">cover</span>...</h1>
                <span class="text-xs">Because if the cover does not impress you what else can?</span>
              </div>
            </div>
          </div>

          <!-- Describition  -->

          <div class="text-white flex flex-col gap-4">
            <div class="">
              <p class="text-2xl text-white font-bold">I'm a frontend Developer.I</p>
              <p class="text-white">Currently, I'm a Software Engineer at</p>
            </div>
            <div class="">
              <p class="font-light text-lg ">A self-taught UI/UX designer, functioning in the industry
                for 3+ years now.
                I make meaningful and delightful digital products that create an equilibrium
                between user needs and business goals.
              </p>
            </div>

          </div>
        </div>
        <!-- working experience -->
        <div id="about">
          <div class="about-radical">
            <div class="flex flex-col gap-3 max-sm:mt-0 max-sm:px-2">
              <h1 class="text-white text-3xl mb-4">Work Experience</h1>
              <div class="flex flex-col gap-4">
                <div class="flex gap-4 max-md:flex-col">
                  <AppCard>
                    <div class="flex p-2 gap-2">
                      <img src="@/assets/images/card1.svg" alt="loading" width="96">
                      <div class="flex flex-col text-white gap-2">
                        <h4 class="text-xl font-bold">CIB on the Mobile</h4>
                        <p class="text-[10px]">Take your client onboard seamlessly by our amazing
                          tool of digital onboard process</p>
                        <button class=" border-blue-300 bg-blue-300 py-2 w-2/5 text-[9px] rounded-xl">LEARN
                          MORE</button>
                      </div>

                    </div>
                  </AppCard>
                  <AppCard>
                    <div class="flex p-2 gap-2">
                      <img src="@/assets/images/card2.svg" alt="loading" width="96">
                      <div class="flex flex-col text-white gap-2">
                        <h4 class="text-xl font-bold">CIB on the Mobile</h4>
                        <p class="text-[10px]">Take your client onboard seamlessly by our amazing
                          tool of digital onboard process</p>
                        <button class=" border-blue-300 bg-blue-300 py-2 w-2/5 text-[9px] rounded-xl">LEARN
                          MORE</button>
                      </div>

                    </div>
                  </AppCard>
                </div>
                <div class="flex gap-4 max-md:flex-col">
                  <AppCard>
                    <div class="flex p-2 gap-2">
                      <img src="@/assets/images/card3.svg" alt="loading" width="96">
                      <div class="flex flex-col text-white gap-2">
                        <h4 class="text-xl font-bold">CIB on the Mobile</h4>
                        <p class="text-[10px]">Take your client onboard seamlessly by our amazing
                          tool of digital onboard process</p>
                        <button class=" border-blue-300 bg-blue-300 py-2 w-2/5 text-[9px] rounded-xl">LEARN
                          MORE</button>
                      </div>

                    </div>
                  </AppCard>
                  <AppCard>
                    <div class="flex p-2 gap-2">
                      <img src="@/assets/images/card4.svg" alt="loading" width="96">
                      <div class="flex flex-col text-white gap-2">
                        <h4 class="text-xl font-bold">CIB on the Mobile</h4>
                        <p class="text-[10px]">Take your client onboard seamlessly by our amazing
                          tool of digital onboard process</p>
                        <button class=" border-blue-300 bg-blue-300 py-2 w-2/5 text-[9px] rounded-xl">LEARN
                          MORE</button>
                      </div>

                    </div>
                  </AppCard>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- skills  -->
        <div class="flex flex-col gap-4 text-center h-full">
          <p class="text-white text-2xl font-bold">I'm currently looking to join a <span
              class="text-blue-200">cross-functional</span> team <br> <span class=" text-[.7em] font-medium">that values
              improving people's lives through accessible design </span></p>
          <div class="skills">
            <img src="@/assets/images/backGround.svg" alt="loading">
          </div>
        </div>
      </div>
    </div>

  </NuxtLayout>
</template>
<style scoped>
#about {
  /* border-top: #763CAC 2px solid; */
  width: 100%;
  display: flex;
  flex-direction: column;
  /* justify-items: center;
  align-items: center; */
  /* height: 100vh; */
}

.radical-bg {
  background: radial-gradient(50% 50% at 50% 50%, #763CAC 0%, rgba(50, 15, 133, 0) 100%);
  /* width: 280px; */

}

/* .arrow {
  background-image: url("@/assets/images/Arrow.svg");
  background-repeat: no-repeat;
} */
.cover {
  border: 1px solid #FFFFFF;
  transform: rotate(-4.74deg);
  box-sizing: border-box;
  border-radius: 50%;
}

.about-radical {
  background: radial-gradient(50% 50% at 50% 50%, #763CAC 0%, rgba(50, 15, 133, 0) 100%);
  top: 0;
}

/* .skills{
  height: 500;
  background-image: url('@/assets/images/backGround.svg');
  background-repeat: no-repeat;
  background-color: none;
} */
</style>
