<script setup>
  import { useReward } from 'vue-rewards'
  import { watch, ref } from 'vue'
  const { reward: confettiReward, isAnimating: isConfettiAnimating } = useReward('some-id', 'confetti');
  const { reward: emojiReward, isAnimating: isEmojiAnimating } = useReward('some-id', 'emoji');

  const start = ref(false)

  const thorwReward = () => {
    start.value = !start.value;
    
    if(start.value){
        confettiReward();    
    }
  }

  watch(isConfettiAnimating, (newVal) => {
    if (newVal === false) {
        if(start.value){
            emojiReward();
        }
    }
  });
  
  watch(isEmojiAnimating, (newVal) => {
    if (newVal === false) {
        if(start.value){
        confettiReward();
        }
    }
  });
  
</script>

<template>
  <span id="some-id" @click="thorwReward"> Let's celebrate! </span>
  
</template>