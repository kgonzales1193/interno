<template>
  <section class="news mt-[80px] xl:mt-[150px] relative z-20">
    <div v-motion :initial="{ opacity: 0, y: 100 }" :visibleOnce="{
      opacity: 1, y: 0, transition: {
        duration: 1500,
        delay: 500,
        type: 'keyframes',
        ease: 'easeInOut',
      },
    }" class="container mx-auto px-0">
      <!-- Text -->
      <div class="max-w-[810px] mx-auto text-center mb-[52px]">
        <h2 class="news__title h2 mb-3">Articles & News</h2>
        <p class="news__subtitle">
          It is a long established fact that a reader will be distracted by the of readable content of a page when
          lookings at its layouts the points of using.
        </p>
      </div>
      <!-- Grid -->
      <div class="news__grid grid grid-cols-1 xl:grid-cols-3 gap-[27px]">
        <!-- Grid Item -->
        <div
          class="news__item w-full max-w-[382px] h-[520px] border-primary/20 rounded-[62px] p-[20px] hover:bg-accent-secondary transition-all group cursor-pointer mx-auto xl:mx-0">
          <img class="mb-5" src="../assets/news/01.png" alt="news" />
          <div class="flex flex-col gap-[30px]">
            <h3 class="h3">
              Let’s Get Solution For Building Construction Work
            </h3>
            <div class="flex items-center justify-between">
              <p class="text-base">22 June, 2024</p>
              <button
                class="bg-accent-secondary w-[52px] h-[52px] rounded-full group-hover:bg-white transition-all flex items-center justify-center">
                <ChevronRight :size="30" class="text-primary pl-1" />
              </button>
            </div>
          </div>
        </div>
        <!-- Grid Item -->
        <div
          class="news__item w-full max-w-[382px] h-[520px] border-primary/20 rounded-[62px] p-[20px] hover:bg-accent-secondary transition-all group cursor-pointer mx-auto xl:mx-0">
          <img class="mb-5" src="../assets/news/02.png" alt="news" />
          <div class="flex flex-col gap-[30px]">
            <h3 class="h3">
              Title: Low Cost Latest Invented Interior Designing
              Ideas
            </h3>
            <div class="flex items-center justify-between">
              <p class="text-base">24 June, 2024</p>
              <button
                class="bg-accent-secondary w-[52px] h-[52px] rounded-full group-hover:bg-white transition-all flex items-center justify-center">
                <ChevronRight :size="30" class="text-primary pl-1" />
              </button>
            </div>
          </div>
        </div>
        <!-- Grid Item -->
        <div
          class="news__item w-full max-w-[382px] h-[520px] border-primary/20 rounded-[62px] p-[20px] hover:bg-accent-secondary transition-all group cursor-pointer mx-auto xl:mx-0">
          <img class="mb-5" src="../assets/news/03.png" alt="news" />
          <div class="flex flex-col gap-[30px]">
            <h3 class="h3">
              Best For Any Office & Business Interior
              Solution
            </h3>
            <div class="flex items-center justify-between">
              <p class="text-base">28 June, 2024</p>
              <button
                class="bg-accent-secondary w-[52px] h-[52px] rounded-full group-hover:bg-white transition-all flex items-center justify-center">
                <ChevronRight :size="30" class="text-primary pl-1" />
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ChevronRight } from 'lucide-vue-next'
</script>

