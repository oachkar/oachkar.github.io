<template>
  <section id="clients">
    <h2>Clients</h2>
    <div class="clients-imgs" style="">
      <a href="https://cls.health/" target="_blank">
        <img src="@/content/CLS_Logo_Main_Stacked.png" />
      </a>
      <a href="https://www.tamu.edu/" target="_blank">
        <img src="@/content/TAM-Horz-Maroon.png" />
      </a>
    </div>
  </section>
</template>
<style scoped>
.clients-imgs {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 2%;
}

.clients-imgs img {
  height: 8rem;
  padding: 1rem;
  background-color: whitesmoke;
  opacity: 0.85;
  transition: 0.25s ease;
}
.clients-imgs img:hover {
  opacity: 1;
  scale: 1.05;
}

@media (max-width: 800px) {
  .clients-imgs {
    flex-direction: column;
    width: 100%;
  }

  .clients-imgs img {
    height: 6rem;
    opacity: 1;
    margin-bottom: 1rem;
  }
}
</style>
