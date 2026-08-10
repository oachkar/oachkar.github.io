<script setup>
defineProps({
  title: {
    type: String,
    required: true,
  },
  link: {
    type: String,
    required: true,
  },
  link_label: {
    type: String,
    required: true,
  },
  img: {
    type: String,
    required: false,
  },
})
</script>

<template>
  <div class="card">
    <img :src="img" class="card-img-top" :alt="title" v-if="img" />
    <div class="card-body">
      <div style="display: flex; gap: 0.5rem; flex-direction: column">
        <h5 class="card-title">{{ title }}</h5>
        <p class="card-text">
          <slot></slot>
        </p>
      </div>
      <a :href="link" target="_blank" class="btn"> Visit {{ link_label }} </a>
    </div>
  </div>
</template>

<style>
.card-img-top {
  transition: 0.25s;
  height: 13rem;
}
.card-img-top:hover {
  transition: 0.25s;
  scale: 110%;
  border-radius: 0.5rem;
}

.card {
  width: 30%;
  min-width: 20rem;
  border: none;
  background-color: var(--color-background);
  color: var(--color-text);
}

.card .card-body {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  gap: 1rem;
}

.btn {
  background-color: hsla(160, 100%, 37%, 1);
  color: white;
}
.btn:hover {
  background-color: rgb(0, 178, 119);
  color: white;
}

@media (max-width: 800px) {
  .card-container {
    flex-direction: column;
    align-items: center;
  }

  .card {
    width: 100%;
    min-width: auto;
  }
  .card-img-top {
    height: auto;
  }
}
</style>
