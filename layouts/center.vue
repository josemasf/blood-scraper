<template>
<div class="slidev-layout container ">
    <div class="absolute inset-0 z-0 opacity-10  ">
      <Background />
    </div>
    
    <div class="mt-10 z-2">
      <slot />
    </div>
</div>
</template>

<script setup>
import Background from '../assets/svg/Background.vue';

</script>