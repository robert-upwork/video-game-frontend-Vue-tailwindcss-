<template>
  <div class="w-full flex justify-center">
    <nav
      class="w-full flex items-center justify-between flex-wrap p-2 max-w-1600 px-40"
    >
      <div class="flex items-center flex-shrink-0 text-white">
          <router-link to="/games" class="font-semibold text-2xl xl:text-3xl tracking-tight mr-5">iPUPPET</router-link>
          <a href="#" class="h-full items-center mx-2 xl:mx-4 text-lg xl:text-xl flex">
            <img :src="require('@/assets/images/nav/home.png')" class="px-2 h-5 xl:h-6"/>
            <!-- <span class="hidden lg:flex">主页</span> -->
            <span class="flex">HOME</span>
          </a>
          <router-link to="/games" class="h-full items-center mx-2 text-lg xl:text-xl relative flex">
            <img :src="require('@/assets/images/nav/grid.png')" class="px-2 h-5 xl:h-6"/> 
            <!-- <span class="flex">软件</span> -->
            <span class="flex">SOFTWARE</span>
            <div class="absolute min-w-full h-3px rounded-full -bottom-18 xl:-bottom-19" style="background-color: #84E4A3;"/>
          </router-link>
      </div>
      <div class="relative">
          <input class="bg-whitegray rounded-full w-56 p-2 pl-10 text-black" :style="'border-width: 0; outline-width: 0'"/>
          <div class="absolute flex items-center h-full" :style="'left:0; top:0'">
            <img :src="require('@/assets/images/nav/search.png')" class="p-2"/>
          </div>
        </div>
      <div class="flex ml-32 xl:ml-56">
        <a href="#" class="">
          <img :src="require('@/assets/images/nav/lightning.png')" class="pr-2 h-5 xl:h-6"/>
        </a>
        <a href="#" class="ml-2">
          <img :src="require('@/assets/images/nav/alarm.png')" class="pr-2 h-5 xl:h-6"/>
        </a>
        <a href="#" class="ml-2">
          <img :src="require('@/assets/images/nav/signal.png')" class="pr-2 h-5 xl:h-6"/>
        </a>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Nav"
};
</script>