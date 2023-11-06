<template>
  <div class="slidev-layout container">
    <div class="absolute inset-0 z-1  ">
      <img
        src="../assets/bg-content.png"
        alt=""
        
      />
    </div>
    
    <div class="mt-10 z-2">
      <p class="text-center text-5xl">Contenido</p>
      <div class="grid grid-cols-3 gap-4 text-white mt-10">
        <div>
          <slot name="first-col" />
        </div>
        <div>
          <slot name="second-col" />
        </div>
        <div>
          <slot name="third-col" />
        </div>
      </div>
    </div>
  </div>
  
</template>

<script setup >



</script>

<style lang="postcss" scoped>
.intro{
  color: #222224;
}
</style>
