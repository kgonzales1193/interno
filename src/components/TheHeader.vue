<template>
  <header class="sticky top-0 h-[90px] shadow-xl z-30 bg-white">
    <div class="container mx-auto flex justify-between h-full items-center">
      <router-link to="/">
        <img src="../assets/logo.svg" alt="logo">
      </router-link>
      <nav>
        <!-- nav mobile trigger -->
        <div class="cursor-pointer lg:hidden" id="nav-trigger-btn" ref="navTriggerBtn">
          <IconMenu class="text-primary" />
        </div>
        <ul
          class="fixed w-full h-0 p-0 bg-white overflow-hidden border-t top-[90px] left-0 right-0 flex flex-col gap-4 lg:relative lg:flex-row lg:p-0 lg:top-0 lg:border-none lg:h-full transition-all duration-300"
          id="nav-menu" ref="navMenu">
          <li>
            <a href="#">Home</a>
          </li>
          <li>
            <a href="#">About</a>
          </li>
          <li>
            <a href="#">Testimonials</a>
          </li>
          <li>
            <a href="#">Our Work</a>
          </li>
          <li>
            <a href="#">News</a>
          </li>
          <li>
            <a href="#">Contact</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import IconMenu from './icons/IconMenu.vue';

const navTriggerBtn = ref(null);
const navMenu = ref(null);

onMounted(() => {
  navTriggerBtn.value.addEventListener('click', () => {
    if (navMenu.value) {
      navMenu.value.classList.toggle('nav-is-open');
    }
  });
});


</script>
