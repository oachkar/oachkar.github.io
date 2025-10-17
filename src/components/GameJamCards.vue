<script>
import GameJamCard from './reusables/GameJamCard.vue'

export default {
  components: { GameJamCard },
}
</script>

<template>
  <section id="projects" class="c-invisible">
    <h2>Game Jam Projects</h2>
    <p>
      I've been involved in a number of game jams in which I worked very closely with team members
      to produce a fully featured demo within a short time. My contributions to these projects
      consisted of programming, systems design, UI and mechanical implementation. For
      <i>Pepper Hermit</i>, I also worked on most of the art.
    </p>
    <p>
      A lot of work goes into game development, and it's very rare that one person has all the
      skills to do it well alone. These projects are a testament to my ability to work in teams and
      communicate with artists, composers, and designers to work collaboratively towards a single
      vision, as well as my ability to realistically manage a project within a strict deadline.
    </p>
    <div class="game-jam-cards">
      <!-- Gelatoss Card -->
      <GameJamCard
        title="Gelatoss!"
        desc="A couch competitive game of high velocity slime splitting."
        link="https://fresh4.itch.io/gelatoss"
        img="https://img.itch.zone/aW1nLzE0Nzk4MTYzLnBuZw==/315x250%23c/zRYdQy.png"
        dl
      />

      <!-- Pepper Hermit Card -->
      <GameJamCard
        title="Pepper Hermit"
        desc="Take on the role of a secret cabal's researcher to develop the ultimate capsaicin potion known to man!"
        link="https://fresh4.itch.io/pepper-hermit"
        img="https://img.itch.zone/aW1nLzE3MTMwMzE4LnBuZw==/315x250%23c/0EpDil.png"
      />

      <!-- Mount Bowlympus Card -->
      <GameJamCard
        title="Mount Bowlympus"
        desc="Roll, smash, and soar through this Synthwave inspired open leveled arcade bowler!"
        link="https://fresh4.itch.io/hyperbowl"
        img="https://img.itch.zone/aW1nLzE5NjE1NTMxLnBuZw==/315x250%23c/fwR9TC.png"
      />

      <!-- The Great Eggscape Card -->
      <GameJamCard
        title="The Great Eggscape"
        desc="Get cracking through this eggcelent platforming eggsperience."
        link="https://fresh4.itch.io/egg"
        img="https://img.itch.zone/aW1nLzIyMzk3NzM5LnBuZw==/315x250%23c/O0j%2BaB.png"
      />

      <!-- Over/Under Card -->
      <GameJamCard
        title="Over/Under"
        desc="Every boon has a price."
        link="https://fresh4.itch.io/over-under"
        img="https://img.itch.zone/aW1nLzIyOTMzNTI1LnBuZw==/315x250%23c/uVSBsD.png"
      />

      <!-- PopRocks card -->
      <GameJamCard
        title="PopRocks"
        desc="Ready to rock? Get poppin' to this cozy lo-fi rhythm game."
        link="https://fresh4.itch.io/poprocks"
        img="https://img.itch.zone/aW1nLzIzMjEzNjQyLnBuZw==/315x250%23c/zos1gR.png"
      />

      <!-- Gore Factory card -->
      <GameJamCard
        title="Gore Factory 凌迟厂"
        desc="Please remember to eat all your rice."
        link="https://fresh4.itch.io/gorefactory"
        img="https://img.itch.zone/aW1nLzIzNjQ1NTY3LnBuZw==/315x250%23c/Be8yQH.png"
      />
    </div>
    <br />
  </section>
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
