<template>
  <section class="brands mt-[80px] xl:mt-[150px] relative z-20">
    <div v-motion :initial="{ opacity: 0, y: 100 }" :visibleOnce="{
      opacity: 1, y: 0, transition: {
        duration: 1500,
        type: 'keyframes',
        ease: 'easeInOut',
      },
    }" class="container mx-auto">
      <div class="flex flex-col xl:flex-row justify-between items-center gap-12">
        <img class="brands__img" src="../assets/brands/01.svg" alt="brand">
        <img class="brands__img" src="../assets/brands/02.svg" alt="brand">
        <img class="brands__img" src="../assets/brands/03.svg" alt="brand">
        <img class="brands__img" src="../assets/brands/04.svg" alt="brand">
        <img class="brands__img" src="../assets/brands/05.svg" alt="brand">
      </div>
    </div>
  </section>
</template>

<script setup>

</script> 
