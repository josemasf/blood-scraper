<template>
  <div class="slidev-layout intro container">
    <div class="absolute inset-0 z-1 bg-[#F6F6F6] ">
      <div class="w72 h72 p-20 absolute z1 top-42 left-[17%] rounded-full bg-gray-200 drop-shadow-md z-2">
        <slot name="icon" />          
      </div>
      
      <Points class="absolute z0 right-[5%] top-[-5%] w-75" />
      <Circles class="absolute z0 left-[-35%] top-[-100%] w-150" />
      <AidaCircle class="w48 h48 absolute z1 top-72 left-[37%]" />
      <!--<img
        src="../assets/bg-intro-v2.png"
        alt=""
        :class="$slidev.nav.clicks ? 'opacity-50' : 'opacity-80'"
      />-->
    </div>
    <div class="relative z-2">
      <div class="absolute bottom-0 right-0 w-[33%]">
        <slot />
      </div>
    </div>
  </div>
</template>

<script setup >
import AidaCircle from '../assets/svg/AidaCircle.vue'
import Circles from '../assets/svg/Circles.vue';
import Points from '../assets/svg/Points.vue';

import { IconSlideshow} from '@tabler/icons-vue'

</script>

<style lang="postcss" scoped>
.intro{
  color: #222224;
}
</style>
