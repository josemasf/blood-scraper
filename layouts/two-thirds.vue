<template>
  <div class="slidev-layout container ">
    <div class="mt-10 z-2">
      <p class="text-center text-2xl"><slot /></p>
      <div class="grid grid-cols-3 gap-4 text-white mt-10">
        <div class="col-span-2">
          <slot name="first-col" />
        </div>
        <div class="border rounded p-5">
          <slot name="second-col" />
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
