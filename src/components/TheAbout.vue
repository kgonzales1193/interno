<template>
  <section class="about mt-[80px] xl:mt-[200px] relative z-20">
    <div class="container mx-auto xl:p-0">
      <div class="flex flex-col xl:flex-row text-center xl:text-left justify-between items-center gap-8 xl:gap-[74px]">
        <!-- Text -->
        <div v-motion :initial="{ opacity: 0, x: -100 }" :visibleOnce="{
          opacity: 1, x: 0, transition: {
            duration: 1500,
            type: 'keyframes',
            ease: 'easeInOut',
          },
        }"
          class="flex-1 order-2 xl:order-none max-w-xl xl:max-w-[410px] flex flex-col items-center xl:items-start gap-8">
          <h2 class="h2">We Create The Art Of Stylish Living Stylishly</h2>
          <p class="">It is a long established fact that a reader will be distracted by the of readable
            content of a page
            when lookings at its layouts the points of using
            that it has a more-or-less normal.</p>
          <!-- Phone -->
          <div class="flex items-center justify-center xl:justify-start gap-4">
            <div class="bg-accent/15 w-[93px] h-[93px] rounded-full flex justify-center items-center">
              <IconPhoneFill class="text-accent text-4xl" />
            </div>
            <div class="text-left">
              <div class="text-2xl font-bold">0985358462</div>
              <div>Call Us Anytime</div>
            </div>
          </div>
          <!-- Button -->
          <button class="btn btn-primary capitalize">
            Get free estimation
            <IconArrowRightLine class="text-accent" />
          </button>
        </div>

        <!-- Image -->
        <div v-motion :initial="{ opacity: 0, x: 100 }" :visibleOnce="{
          opacity: 1, x: 0, transition: {
            duration: 1500,
            type: 'keyframes',
            ease: 'easeInOut',
          },
        }" class="about__img order-1 xl:order-none max-w-[453px] mx-auto xl:max-w-none xl:mx-0">
          <img src="../assets//about/img.png" alt="">
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import IconArrowRightLine from './icons/IconArrowRightLine.vue';
import IconPhoneFill from './icons/IconPhoneFill.vue';
</script>
