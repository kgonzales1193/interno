<template>
  <section class="testimonial mt-[80px] xl:mt-[200px] relative z-20">
    <div v-motion :initial="{ opacity: 0, y: 100 }" :visibleOnce="{
      opacity: 1, y: 0, transition: {
        duration: 1500,
        type: 'keyframes',
        ease: 'easeInOut',
      },
    }" class="testimonial__bg container mx-auto bg-accent-secondary rounded-[70px] px-6">
      <div class="flex flex-col items-center pt-[88px] pb-[110px]">
        <h2 class="h2 mb-9 text-center">
          What clients say...
        </h2>
      </div>
      <!-- Slider -->
      <div class="w-full">
        <swiper :modules="[Pagination]" :breakpoints="{
          1200: {
            slidesPerView: 3,
          },
          960: {
            slidesPerView: 2,
          },
          320: {
            slidesPerView: 1,
          },
        }" :space-between="20" :pagination="{ clickable: true }" class="testimonial__slider swiper h-[400px]">
          <swiper-slide class="swiper-slide">
            <div
              class="testimonial__item w-full max-w-[450px] h-[340px] bg-white rounded-[30px] flex flex-col justify-center p-9 mx-auto">
              <div class="flex gap-4 mb-6">
                <img src="../assets/testimonial/01.png" alt="">
                <div>
                  <h3 class="h3">Nattasha Mith</h3>
                  <div>Greenville, USA</div>
                </div>
              </div>
              <p>
                Lorem Ipsum is simply dummy
                text of the typesetting industry.
                Ipsum has been.
              </p>
            </div>
          </swiper-slide>
          <swiper-slide class="swiper-slide">
            <div
              class="testimonial__item w-full max-w-[450px] h-[340px] bg-white rounded-[30px] flex flex-col justify-center p-9 mx-auto">
              <div class="flex gap-4 mb-6">
                <img src="../assets/testimonial/02.png" alt="">
                <div>
                  <h3 class="h3">Jessica White</h3>
                  <div>Oak Ridge, USA</div>
                </div>
              </div>
              <p>
                Lorem Ipsum is simply dummy
                text of the typesetting industry.
                Ipsum has been.
              </p>
            </div>
          </swiper-slide>
          <swiper-slide class="swiper-slide">
            <div
              class="testimonial__item w-full max-w-[450px] h-[340px] bg-white rounded-[30px] flex flex-col justify-center p-9 mx-auto">
              <div class="flex gap-4 mb-6">
                <img src="../assets/testimonial/03.png" alt="">
                <div>
                  <h3 class="h3">Mike Davis</h3>
                  <div>Berlin, Germany</div>
                </div>
              </div>
              <p>
                Lorem Ipsum is simply dummy
                text of the typesetting industry.
                Ipsum has been.
              </p>
            </div>
          </swiper-slide>
          <swiper-slide class="swiper-slide">
            <div
              class="testimonial__item w-full max-w-[450px] h-[340px] bg-white rounded-[30px] flex flex-col justify-center p-9 mx-auto">
              <div class="flex gap-4 mb-6">
                <img src="../assets/testimonial/04.png" alt="">
                <div>
                  <h3>Olivia Wilson</h3>
                  <div>Blue Ridge, France</div>
                </div>
              </div>
              <p>
                Lorem Ipsum is simply dummy
                text of the typesetting industry.
                Ipsum has been.
              </p>
            </div>
          </swiper-slide>
        </swiper>
      </div>
    </div>
  </section>
</template>

<script setup>
// import Swiper core and required modules
import { Pagination } from 'swiper/modules';

// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/pagination';


</script>
