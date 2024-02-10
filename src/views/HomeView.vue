<script setup>
import TheAbout from '@/components/TheAbout.vue';
import TheBrands from '@/components/TheBrands.vue';
import TheContact from '@/components/TheContact.vue';
import TheFooter from '@/components/TheFooter.vue';
import TheHero from '@/components/TheHero.vue';
import TheNews from '@/components/TheNews.vue';
import TheStats from '@/components/TheStats.vue';
import TheSteps from '@/components/TheSteps.vue';
import TheTestimonial from '@/components/TheTestimonial.vue';
import TheWork from '@/components/TheWork.vue';


</script>

<template>
  <main class="max-w-[1920px] mx-auto bg-white overflow-hidden">
    <!-- Grid BG Image -->
    <div class="xl:bg-grid xl:bg-center xl:bg-repeat-y fixed inset-0 z-10"></div>
    <!-- Hero -->
    <TheHero />
    <!-- Steps -->
    <TheSteps />
    <!-- About -->
    <TheAbout />
    <!-- Testimonial -->
    <TheTestimonial />
    <!-- Brands -->
    <TheBrands />
    <!-- Works -->
    <TheWork />
    <!-- Stats -->
    <TheStats />
    <!-- News -->
    <TheNews />
    <!-- Contact -->
    <TheContact />
    <!-- Footer -->
    <TheFooter />
  </main>
</template>
