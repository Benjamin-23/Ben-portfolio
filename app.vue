<script lang="ts" setup>
const runtimeConfig = useRuntimeConfig()
const appConfig = useAppConfig()
function makecall (){
  let number = "+254716613981"
  let whatsappApiUrl= `https://wa.me/${number}`
  window.open( whatsappApiUrl, "_blank")
  
}

</script>
<template>
  <NuxtLayout>
    <div class="flex mt-12 w-full justify-center mb-8">
      <div class="flex flex-col gap-12 max-w-[60%] max-md:max-w-[80%]">
        <!-- Home page -->
        <!--  -->
        <div class="flex flex-col w-full gap-6 h-[85vh] justify-center max-md:h-full">
          <div class="flex max-md:flex-col">
            <div class="radical-bg justify-center items-center flex">
              <img src="@/assets/images/profile.svg" alt="loading" class="w-60 cursor-grabbing max-md:w-48 hover:skew-y-2">
            </div>
            <div
              class="flex-col  gap-10 flex ml-[-20px] text-white mt-4 max-sm:gap-6 max-sm:mt-3 max-md:items-center max-md:px-4">
              <div class="flex w-full gap-6 justify-evenly">
                <p class=" w-full text-m">Hello! I Am <span class=" text-blue-200">Benjamin Kitonga</span></p>
              </div>
              <div class="flex flex-col gap-2">
                <p class="font-[Preahvihear, poppins] text-sm underline">A Designer who</p>
                <h1 class="font-bold text-[2em] max-sm:text-[1.5em]">Judges a book <br> by its <span
                    class="text-blue-200 cover p-1 text-ellipsis">cover</span>...</h1>
                <span class="text-xs">Because if the cover does not impress you what else can? 😂 </span>
                <span class="text-sm animate-bounce text-red-500 underline decoration-pink-500">Kidding 🔞</span>

              </div>
            </div>
          </div>

          <!-- Describition  -->

          <div class="text-white flex flex-col gap-4">
            <div class="">
              <p class="text-2xl text-white font-bold">I'm a frontend Developer.I</p>
              <p class="text-white text-lg md:text-sm ">Currently, I'm a Software Engineer at Artemis</p>
            </div>
            <div class=" flex flex-col gap-8">
              <p class="font-light text-md max-md:text-base">A self-taught UI/UX designer, 
                functioning in the industryfor 3+ years now.
                I make meaningful and delightful digital products that create an equilibrium
                between user needs and business goals.
                I'm solving your problems with code and create the best product
              </p>
             <button @click="makecall()" class=" bg-blue-200 border-none w-1/4 py-2 rounded-md max-md:w-1/2 cursor-pointer text-md ring ring-purple-600 ring-offset-4 outline-none dark:ring-offset-blue-100">Make a call</button>
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
                    <div class="flex p-2 gap-2 max-md:gap-1">
                      <img src="@/assets/images/card1.svg" alt="loading" class=" w-20 max-md:w-16">
                      <div class="flex flex-col text-white gap-2">
                        <h4 class="text-xl font-bold max-md:text-lg">Bulk SMS Project</h4>
                        <p class="text-[10px]">A sms platform , Help organizations to communicate 
                          with there customer with only one tap 
                        </p>
                        <button
                          class=" border-blue-300 bg-blue-300 py-2 w-2/5 text-[9px] rounded-xl max-md:text-[7.5px]">LEARN
                          MORE</button>
                      </div>

                    </div>
                  </AppCard>
                  <AppCard>
                    <div class="flex p-2 gap-2 max-md:gap-1">
                      <img src="@/assets/images/card2.svg" alt="loading" class=" w-20 max-md:w-16">
                      <div class="flex flex-col text-white gap-2">
                        <h4 class="text-xl font-bold max-md:text-lg">Teleporting Websites</h4>
                        <p class="text-[10px]">Connecting Websites with the current AI technology and
                          Creating a robotic static pages. 
                        </p>
                        <button
                          class=" border-blue-300 bg-blue-300 py-2 w-2/5 text-[9px] rounded-xl max-md:text-[7.5px]">LEARN
                          MORE</button>
                      </div>

                    </div>
                  </AppCard>
                </div>
                <div class="flex gap-4 max-md:flex-col">
                  <AppCard>
                    <div class="flex p-2 gap-2 max-md:gap-1">
                      <img src="@/assets/images/card3.svg" alt="loading" class=" w-20 max-md:w-16">
                      <div class="flex flex-col text-white gap-2">
                        <h4 class="text-xl font-bold max-md:text-lg">Mobile & Desktop Apps</h4>
                        <p class="text-[10px]">Creating with Flutter furnishing with Electron for
                          better experience.Well customized designs  
                        </p>
                        <button
                          class=" border-blue-300 bg-blue-300 py-2 w-2/5 text-[9px] rounded-xl max-md:text-[7.5px]">LEARN
                          MORE</button>
                      </div>

                    </div>
                  </AppCard>
                  <AppCard>
                    <div class="flex p-2 gap-2 max-md:gap-1">
                      <img src="@/assets/images/card4.svg" alt="loading" class=" w-20 max-md:w-16">
                      <div class="flex flex-col text-white gap-2">
                        <h4 class="text-xl font-bold max-md:text-lg">CIB on the Mobile</h4>
                        <p class="text-[10px]">Take your client onboard seamlessly by our amazing
                          tool of digital onboard process</p>
                        <button
                          class=" border-blue-300 bg-blue-300 py-2 w-2/5 text-[9px] rounded-xl max-md:text-[7.5px]">LEARN
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
        <div class="flex flex-col text-center gap-4 max-md:gap-14">
          <p class="text-white text-2xl font-bold max-md:[ text-xl, font-semibold]">I'm currently looking to join a <span
              class="text-blue-200 line-through tracking-wide">cross-functional</span> team <br> <span class=" text-[.7em] font-medium">that values
              improving people's lives through accessible design </span></p>
          <div class="">
            <img src="@/assets/images/backGround.svg" alt="loading" class=" w-84 max-md:scale-[1.2]" >
          </div>
        </div>
        <!-- projects  -->
        <div id="lab"></div>
        <div class=" my-4 flex flex-col gap-12 -z-10 ">
          <div class="flex">
            <div class="flex flex-col text-white gap-2 w-3/5 z-10 max-md:w-full">
              <div class="">
                <span class=" text-xs text-blue-200 font-medium">Featured Project</span>
                <h4 class=" text-lg font-bold animate-pulse">Example Project</h4>
              </div>

              <div class=" bg-blue-100 rounded-2xl">
                <p class=" text-xs px-2  py-4 radical-card">
                  A web app for visualizing personalized Spotify data. View your
                  top artists, top tracks, recently played tracks, and detailed audio
                  information about each track. Create and save new playlists of
                  recommended tracks based on your existing playlists and more.
                </p>
              </div>
              <div class="flex gap-2 ">
                <img  src="@/assets/images/icon-park-solid_click.svg" alt="" class=" w-4 animate-spin">
                <img src="@/assets/images/icon-park-solid_click.svg" alt="" class=" w-4 animate-spin">
              </div>
            </div>
            <!-- project image -->
            <div class="project-radical w-2/5 bg-repeat-x bg-center ml-[-40px] flex justify-center max-md:w-full">
              <img src="@/assets/images/project2.svg " alt="loading " class=" hover:backdrop-blur">
            </div>
          </div>

          <div class="flex">
            <!-- project image -->
            <div class="project-radical w-2/5 bg-repeat-x bg-center flex justify-center max-md:w-full">
              <img src="@/assets/images/project2.svg" alt="loading">
            </div>
            <div class="flex flex-col text-white gap-2 w-3/5 z-10 items-end ml-[-40px] max-md:w-full">
              <div class=" text-right">
                <span class="text-blue-200 font-medium text-xs">Featured Project</span>
                <h4 class=" font-bold text-lg">Example Project</h4>
              </div>

              <div class=" bg-blue-100 rounded-2xl">
                <p class=" text-xs px-2 py-4 radical-card">
                  A web app for visualizing personalized Spotify data. View your
                  top artists, top tracks, recently played tracks, and detailed audio
                  information about each track. Create and save new playlists of
                  recommended tracks based on your existing playlists and more.
                </p>
              </div>
              <div class="flex gap-2">
                <img src="@/assets/images/icon-park-solid_click.svg" alt="" class="w-4 animate-spin">
                <img src="@/assets/images/icon-park-solid_click.svg" alt="" class="w-4 animate-spin">
              </div>
            </div>
          </div>
        </div>
        <!-- contact details -->
        <div class="flex flex-col gap-6 text-white w-[75%]">
          <h2 class="">Contact</h2>
          <div class="flex flex-col gap-2">
            <p class="text-sm">I'm currently looking to join a cross-functional team that values improving people's
              lives
              through accessible design. or have a project in mind? Let's connect.</p>
            <p class="text-sm">kitongabenja34@gmail.com</p>
          </div>
          <div class="flex gap-4">
            <img src="@/assets/images/ig.svg" alt="">
            <img src="@/assets/images/link.svg" alt="">
            <img src="@/assets/images/google.svg" alt="">
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

.project-radical {
  background: radial-gradient(50% 50% at 50% 50%, #763CAC 0%, rgba(50, 15, 133, 0) 100%);
}

.radical-card {
  background: url(.png), radial-gradient(90.16% 143.01% at 15.32% 21.04%, rgba(105, 59, 147, 0.2) 0%, rgba(110, 191, 244, 0.0447917) 77.08%, rgba(70, 144, 213, 0) 100%);
  background-blend-mode: overlay, normal;
  backdrop-filter: blur(40px);
  /* Note: backdrop-filter has minimal browser support */

  border-radius: 14px;
}

/* .skills{
  height: 500;
  background-image: url('@/assets/images/backGround.svg');
  background-repeat: no-repeat;
  background-color: none;
} */
</style>
