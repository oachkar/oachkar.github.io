<script setup>
defineProps({
  title: {
    type: String,
    required: true,
  },
  desc: {
    type: String,
    required: true,
  },
  link: {
    type: String,
    required: true,
  },
  img: {
    type: String,
    required: true,
  },
  alt: {
    type: String,
    required: true,
  },
  dl: {
    type: Boolean,
    required: false,
  },
})
// const props = defineProps(['title', 'desc', 'img', 'alt', 'web'])
</script>

<template>
  <div class="card" style="width: 18rem">
    <img :src="img" class="card-img-top" :alt="title" />
    <div class="card-body">
      <h5 class="card-title">{{ title }}</h5>
      <p class="card-text">{{ desc }}</p>
      <a :href="link" target="_blank" class="btn itch-btn">
        {{ !dl ? 'Play' : 'Download' }} on itch.io
      </a>
    </div>
  </div>
</template>

<style scoped>
.card-img-top {
  transition: 0.25s;
}
.card-img-top:hover {
  transition: 0.25s;
  scale: 110%;
  border-radius: 0.5rem;
}

.itch-btn {
  background-color: #fa5c5c;
  color: #fff;
}

.itch-btn:hover {
  background-color: #e04e4e;
  color: #fff;
}

.game-jam-cards {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 2rem;
}

.game-jam-cards .card .card-body {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.game-jam-cards .card {
  border: none;
  justify-self: center;
}

@media (max-width: 800px) {
  .game-jam-cards {
    grid-template-columns: 1fr;
  }
}
</style>
