<template>
  <section class="work mt-[80px] xl:mt-[150px] relative z-20">
    <div class="container mx-auto xl:px-0">
      <!-- Text -->
      <div v-motion :initial="{ opacity: 0, y: 100 }" :visibleOnce="{
        opacity: 1, y: 0, transition: {
          duration: 1500,
          delay: 500,
          type: 'keyframes',
          ease: 'easeInOut',
        },
      }" class="text-center mb-24">
        <h2 class="work__title h2 mb-4">Follow Our Projects</h2>
        <p class="work__subtitle max-w-3xl mx-auto">It is a long established fact that a reader will be distracted by the
          of readable content of page lookings at
          its layouts points.</p>
      </div>
      <!-- Grid -->
      <div v-motion :initial="{ opacity: 0, y: 100 }" :visibleOnce="{
        opacity: 1, y: 0, transition: {
          duration: 1500,
          delay: 500,
          type: 'keyframes',
          ease: 'easeInOut',
        },
      }" class="work__grid grid grid-cols-1 xl:grid-cols-2 gap-x-[104px] gap-y-[56px]">
        <!-- Item 1 -->
        <div class="w-full max-w-[548px] h-full mx-auto">
          <img class="mb-6" src="../assets/work/01.png" alt="work" />
          <div class="flex justify-between items-center w-full">
            <div>
              <h3 class="h3">Modern Kitchen</h3>
              <p>Decor/Architecture</p>
            </div>
            <button
              class="bg-accent-secondary hover:bg-accent/20 w-[70px] h-[70px] flex items-center justify-center rounded-full">
              <ChevronRight :size="30" class="text-primary pl-1" />
            </button>
          </div>
        </div>
        <!-- Item 2 -->
        <div class="w-full max-w-[548px] h-full mx-auto">
          <img class="mb-6" src="../assets/work/02.png" alt="work" />
          <div class="flex justify-between items-center w-full">
            <div>
              <h3 class="h3">Modern Kitchen</h3>
              <p>Decor/Architecture</p>
            </div>
            <button
              class="bg-accent-secondary hover:bg-accent/20 w-[70px] h-[70px] flex items-center justify-center rounded-full">
              <ChevronRight :size="30" class="text-primary pl-1" />
            </button>
          </div>
        </div>
        <!-- Item 3 -->
        <div class="w-full max-w-[548px] h-full mx-auto">
          <img class="mb-6" src="../assets/work/03.png" alt="work" />
          <div class="flex justify-between items-center w-full">
            <div>
              <h3 class="h3">Modern Kitchen</h3>
              <p>Decor/Architecture</p>
            </div>
            <button
              class="bg-accent-secondary hover:bg-accent/20 w-[70px] h-[70px] flex items-center justify-center rounded-full">
              <ChevronRight :size="30" class="text-primary pl-1" />
            </button>
          </div>
        </div>
        <!-- Item 4 -->
        <div class="w-full max-w-[548px] h-full mx-auto">
          <img class="mb-6" src="../assets/work/04.png" alt="work" />
          <div class="flex justify-between items-center w-full">
            <div>
              <h3 class="h3">Modern Kitchen</h3>
              <p>Decor/Architecture</p>
            </div>
            <button
              class="bg-accent-secondary hover:bg-accent/20 w-[70px] h-[70px] flex items-center justify-center rounded-full">
              <ChevronRight :size="30" class="text-primary pl-1" />
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ChevronRight } from 'lucide-vue-next';
</script>
