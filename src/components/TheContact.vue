<template>
  <section v-motion :initial="{ opacity: 0, y: 100 }" :visibleOnce="{
    opacity: 1, y: 0, transition: {
      duration: 1500,
      delay: 500,
      type: 'keyframes',
      ease: 'easeInOut',
    },
  }" class="contact mt-[80px] xl:mt-[150px] relative z-20">
    <div class="contact__container container mx-auto bg-primary sm:rounded-[70px] py-[80px]">
      <div class="contact__text max-w-[640px] mx-auto text-center">
        <h2 class="h2 text-white mb-4">Do you want to join Interno?</h2>
        <p class="text-white mb-8 max-w-sm xl:max-w-none mx-auto">It is a long established fact will be distracted.</p>
        <button class="btn btn-accent mx-auto">Connect With Us
          <IconArrowRightLine />
        </button>
      </div>
    </div>
  </section>
</template>

<script setup>

import IconArrowRightLine from './icons/IconArrowRightLine.vue';
</script>

