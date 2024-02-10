<template>
  <section
    class="hero h-[640px] xl:h-[840px] bg-hero bg-center lg:bg-cover bg-no-repeat bg-fixed xl:rounded-bl-[290px] relative z-20">
    <div class="container mx-auto h-full flex items-center justify-center xl:justify-start">
      <!-- text -->

      <div v-motion :initial="{ opacity: 0, y: 100 }" :enter="{
        opacity: 1, y: 0, transition: {
          duration: 1500,
          type: 'keyframes',
          ease: 'easeInOut',
        },
      }" class="hero__text w-[567px] flex flex-col items-center text-center xl:text-left lg:items-start">
        <h1 class="h1 mb-8">Let Your Home Be Unique</h1>
        <p class="mb-8">There are many variations of the passages of lorem Ipsum from available,variations of the
          passages.</p>
        <button class="btn btn-primary mx-auto xl:mx-0 capitalize">
          Get free estimation
          <IconArrowRightLine class="text-accent" />
        </button>
      </div>
    </div>
  </section>
</template>

<script setup>
import IconArrowRightLine from './icons/IconArrowRightLine.vue';
</script>
