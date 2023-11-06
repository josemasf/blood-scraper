<template>
    <div class="slidev-layout container">
      <div class="absolute inset-0 z-1  ">
        <img
          src="../assets/bg-order-paper.png"
          alt=""
          
        />
      </div>
      
      <div class="mt-10 z-2">
        <p class="text-center text-3xl text-white">Agenda</p>        
        <slot />
      </div>
      
    </div>
  </template>
  
  <script setup >
  import OrderPaperItem from '../components/OrderPaperItem.vue';
  
  </script>
  
  <style lang="postcss" scoped>
  .intro{
    color: #222224;
  }
  </style>
  