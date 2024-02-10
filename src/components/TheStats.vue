<template>
  <section ref="statsRef" class="stats mt-[80px] xl:mt-[150px] relative z-20 bg-accent-secondary">
    <div class="container mx-auto py-[80px] xl:py-[150px]">
      <div class="grid grid-cols-1 xl:grid-cols-4 gap-12">
        <!-- Grid Item -->
        <div class="stats__item text-center xl:border-r xl:border-accent" data-id="years">
          <h3 class="h1 font-primary text-accent">{{ yearsOfExperience }}</h3>
          <p>Years of Experience</p>
        </div>
        <!-- Grid Item -->
        <div class="stats__item text-center xl:border-r xl:border-accent" data-id="projects">
          <h3 class="h1 font-primary text-accent">{{ projectsCompleted }}</h3>
          <p>Projects Completed</p>
        </div>
        <!-- Grid Item -->
        <div class="stats__item text-center xl:border-r xl:border-accent" data-id="active">
          <h3 class="h1 font-primary text-accent">{{ activeProjects }}</h3>
          <p>Active Projects</p>
        </div>
        <!-- Grid Item -->
        <div class="stats__item text-center" data-id="clients">
          <h3 class="h1 font-primary text-accent">{{ happyClients }}</h3>
          <p>Happy Clients</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from 'vue';

const yearsOfExperience = ref(0);
const projectsCompleted = ref(0);
const activeProjects = ref(0);
const happyClients = ref(0);
const statsRef = ref(null); // Reference to the stats container

// Animation function remains the same
const animateValue = (refValue, endValue, duration = 2000) => {
  let start = 0;
  const end = endValue;
  const startTime = performance.now();

  function update(currentTime) {
    const elapsedTime = currentTime - startTime;
    const progress = Math.min(elapsedTime / duration, 1);
    refValue.value = Math.floor(progress * (end - start) + start);
    if (progress < 1) {
      requestAnimationFrame(update);
    }
  }

  requestAnimationFrame(update);
};

onMounted(() => {
  const observer = new IntersectionObserver(
    (entries, observer) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          const id = entry.target.getAttribute('data-id');
          switch (id) {
            case 'years':
              animateValue(yearsOfExperience, 12);
              break;
            case 'projects':
              animateValue(projectsCompleted, 85);
              break;
            case 'active':
              animateValue(activeProjects, 15);
              break;
            case 'clients':
              animateValue(happyClients, 95);
              break;
          }
          observer.unobserve(entry.target); // Stop observing the element after animating
        }
      });
    },
    {
      threshold: 0.1 // Trigger when 10% of the element is in view
    }
  );

  // Assuming you have a ref="statsRef" on your stats container
  document.querySelectorAll('.stats__item').forEach((el) => {
    observer.observe(el);
  });
});
</script>
