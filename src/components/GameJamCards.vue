<!-- GameJamCards.vue -->
<!-- <script setup></script> -->

<template>
  <div class="game-jam-cards">
    <!-- Gelatoss Card -->
    <div class="card" style="width: 18rem">
      <img
        src="https://img.itch.zone/aW1nLzE0Nzk4MTYzLnBuZw==/315x250%23c/zRYdQy.png"
        class="card-img-top"
        alt="Gelatoss!"
      />
      <div class="card-body">
        <h5 class="card-title">Gelatoss!</h5>
        <p class="card-text">A couch competitive game of high velocity slime splitting.</p>
        <a href="https://fresh4.itch.io/gelatoss" class="btn itch-btn">Download on itch.io</a>
      </div>
    </div>

    <!-- Pepper Hermit Card -->
    <div class="card" style="width: 18rem">
      <img
        src="https://img.itch.zone/aW1nLzE3MTMwMzE4LnBuZw==/315x250%23c/0EpDil.png"
        class="card-img-top"
        alt="Pepper Hermit"
      />
      <div class="card-body">
        <h5 class="card-title">Pepper Hermit</h5>
        <p class="card-text">
          Take on the role of a secret cabal's researcher to develop the ultimate capsaicin potion
          known to man!
        </p>
        <a href="https://fresh4.itch.io/pepper-hermit" class="btn itch-btn"> Play on itch.io </a>
      </div>
    </div>

    <!-- Mount Bowlympus Card -->
    <div class="card" style="width: 18rem">
      <img
        src="https://img.itch.zone/aW1nLzE5NjE1NTMxLnBuZw==/315x250%23c/fwR9TC.png"
        class="card-img-top"
        alt="Mount Bowlympus"
      />
      <div class="card-body">
        <h5 class="card-title">Mount Bowlympus</h5>
        <p class="card-text">
          Roll, smash, and soar through this Synthwave inspired open leveled arcade bowler!
        </p>
        <a href="https://fresh4.itch.io/hyperbowl" class="btn itch-btn"> Play on itch.io </a>
      </div>
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
  display: flex;
  justify-content: space-around;
  flex-wrap: nowrap;
  gap: 2rem;
}

.game-jam-cards .card .card-body {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.game-jam-cards .card {
  border: none;
}

@media (max-width: 800px) {
  .game-jam-cards {
    flex-direction: column;
    align-items: center;
  }
}
</style>
