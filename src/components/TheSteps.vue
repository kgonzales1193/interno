<template>
  <section class="steps mt-[80px] xl:mt-[200px] relative z-20">
    <div class="container mx-auto">
      <!-- GRID -->
      <div v-motion :initial="{ opacity: 0, y: 100 }" :visibleOnce="{
        opacity: 1, y: 0, transition: {
          duration: 1500,
          type: 'keyframes',
          ease: 'easeInOut',
        },
      }" class="grid grid-cols-1 gap-12 xl:grid-cols-3">
        <!-- Step 1 -->
        <div class="steps__step text-center">
          <div class="mb-4">
            <DraftingCompass :size="48" class="text-accent inline-block" />
          </div>
          <h3 class="h3 mb-5">Project Planning</h3>
          <p class="mb-5 max-w-md mx-auto">There are many variations of the passages of lorem Ipsum from available,
            majority.</p>
          <a href="#" class="flex items-center justify-center gap-1 font-medium">Read more
            <IconArrowRightLine class="text-accent" />
          </a>
        </div>
        <!-- Step 2 -->
        <div class="steps__step text-center">
          <div class="mb-4">
            <Wand :size="48" class=" text-accent inline-block" />
          </div>
          <h3 class="h3 mb-5">Gaining Materials</h3>
          <p class="mb-5 max-w-md mx-auto">There are many variations of the passages of lorem Ipsum from available,
            majority.</p>
          <a href="#" class="flex items-center justify-center gap-1 font-medium">Read more
            <IconArrowRightLine class="text-accent" />
          </a>
        </div>
        <!-- Step 3 -->
        <div class="steps__step text-center">
          <div class="mb-4">
            <PencilRuler :size="48" class="text-accent inline-block" />
          </div>
          <h3 class="h3 mb-5">Project Execution</h3>
          <p class="mb-5 max-w-md mx-auto">There are many variations of the passages of lorem Ipsum from available,
            majority.</p>
          <a href="#" class="flex items-center justify-center gap-2 font-medium">Read more
            <IconArrowRightLine class="text-accent" />
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Wand, DraftingCompass, PencilRuler } from 'lucide-vue-next';
import IconCompasses from './icons/IconCompasses.vue';
import IconArrowRightLine from './icons/IconArrowRightLine.vue';

</script>

