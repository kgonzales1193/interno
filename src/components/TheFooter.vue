<template>
  <footer v-motion :initial="{ opacity: 0, y: 100 }" :visibleOnce="{
    opacity: 1, y: 0, transition: {
      duration: 1500,
      delay: 500,
      type: 'keyframes',
      ease: 'easeInOut',
    },
  }" class="footer mt-[80px] xl:mt-[150px] relative z-20">
    <div class="container mx-auto px-0">
      <div class="flex flex-col xl:flex-row xl:gap-[100px] xl:mb-[150px]">
        <div class="footer__item w-full max-w-[400px] mx-auto mb-8 text-center xl:text-left">
          <!-- Logo -->
          <a class="flex justify-center xl:justify-start mb-8" href="#">
            <img src="../assets/logo.svg" alt="logo" />
          </a>
          <p class="mb-8 text-xl">
            It is a long established fact that a reader will be distracted lookings.
          </p>
          <!-- Socials -->
          <ul class="text-primary flex gap-[54px] justify-center xl:justify-start">
            <li>
              <a href="">
                <IconFacebookFill />
              </a>
            </li>
            <li>
              <a href="">
                <IconXFill />
              </a>
            </li>
            <li>
              <a href="">
                <IconInstagramFill />
              </a>
            </li>
            <li>
              <a href="">
                <IconLinkedinFill />
              </a>
            </li>
          </ul>
        </div>
        <div class="flex-1 flex flex-col xl:flex-row text-center xl:text-left gap-12 xl:gap-[100px] xl:justify-end">
          <div class="footer__item">
            <h3 class="h3 mb-3">Pages</h3>
            <ul class="flex flex-col gap-4">
              <li>
                <a href="">About Us</a>
              </li>
              <li>
                <a href="">Testimonials</a>
              </li>
              <li>
                <a href="">Our Work</a>
              </li>
              <li>
                <a href="">News</a>
              </li>
              <li>
                <a href="">Contact</a>
              </li>
            </ul>
          </div>
          <div class="footer__item">
            <h3 class="h3 mb-3">Services</h3>
            <ul class="flex flex-col gap-4">
              <li>
                <a href="">Kitchen</a>
              </li>
              <li>
                <a href="">Living Area</a>
              </li>
              <li>
                <a href="">Bathroom</a>
              </li>
              <li>
                <a href="">Bedroom</a>
              </li>
              <li>
                <a href="">Renovation</a>
              </li>
            </ul>
          </div>
          <div class="footer__item max-w-[260px] mx-auto xl:mx-0">
            <h3 class="h3 mb-3">Contact</h3>
            <div class="flex flex-col gap-6 text-[20px]">
              <p>
                55 East Birchwood Ave. Brooklyn, New York 11201
              </p>
              <p>contact@interno.com</p>
              <p>(123) 456 - 7890</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- Copyright -->
    <p class="footer__copyright text-center text-lg py-10 bg-white xl:border-t">Copyright &copy; Interno 2024. All rights
      reserved.</p>
  </footer>
</template>

<script setup>
import IconFacebookFill from './icons/IconFacebookFill.vue';
import IconXFill from './icons/IconXFill.vue';
import IconInstagramFill from './icons/IconInstagramFill.vue';
import IconLinkedinFill from './icons/IconLinkedinFill.vue';


</script>
