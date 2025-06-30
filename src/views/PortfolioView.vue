<script setup>
import GameJamCards from '@/components/GameJamCards.vue'
import WebsitesCards from '@/components/WebsitesCards.vue'
import Profile from '@/components/ProfileCard.vue'
import { onMounted, onUpdated } from 'vue'
// import ClientsCard from '@/components/ClientsCard.vue'
import AboutCard from '@/components/AboutCard.vue'

const observerOptions = {
  root: null,
  rootMargin: '0px',
  threshold: 0.05,
}

function observerCallback(entries) {
  entries.forEach((entry) => {
    if (entry.isIntersecting) {
      // fade in observed elements that are in view
      entry.target.classList.replace('c-invisible', 'c-visible')
    }
  })
}

function computeFade() {
  const observer = new IntersectionObserver(observerCallback, observerOptions)
  const fadeElms = document.querySelectorAll('.c-invisible')
  fadeElms.forEach((el) => observer.observe(el))
}

onMounted(() => {
  computeFade()
})

onUpdated(() => {
  computeFade()
})
</script>

<template>
  <main>
    <Profile class="c-invisible" />
    <hr />

    <GameJamCards class="c-invisible" />
    <hr />

    <WebsitesCards class="c-invisible" />
    <hr />

    <!-- <ClientsCard class="c-invisible" />
    <hr /> -->

    <AboutCard class="c-invisible" />
  </main>
</template>

<style>
section {
  margin-top: 2rem;
  margin-bottom: 2rem;
  background-color: var(--color-background-soft);
  border: 1px solid var(--color-border);
  border-radius: 0.5rem;
  padding: 1rem;
  padding-bottom: 1rem;
}

section:hover {
  border: 1px solid var(--vt-c-green);
}

.c-invisible {
  opacity: 0;
  transition: 0.5s;
  margin-top: 4rem;
}
.c-visible {
  opacity: 100%;
  transition: 0.5s;
}
</style>
