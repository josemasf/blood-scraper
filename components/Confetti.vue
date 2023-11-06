<script setup>
  import { useReward } from 'vue-rewards'
  import { onMounted } from 'vue'

  const config = {
    startVelocity:10,
    spread:180,
    elementCount:100
    // etc...
    // you can make this reactive instead etc.
  }

  // has to be in onMounted, otherwise the element won't be found.
  // This will trigger the animation immediately.
  
  // or you can trigger the animation onclick
  // I have renamed reward to balloonsReward etc.

  const { reward: balloonsReward, isAnimating: isBalloonsAnimating } = useReward('some-id', 'confetti');
</script>

<template>
  <span id="some-id" @click="balloonsReward"> Let's celebrate! </span>
  
</template>