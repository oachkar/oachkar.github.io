<template>
  <div class="card-container">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">CLS Stream</h5>
        <p class="card-text">
          A web application developed for the multi-speciality clinic CLS Health in Webster, Texas.
          Though it is an internal tool, here is one public facing application. It utilizes React
          and Bootstrap for the front end, and communication with a backend API that hits a
          database, the Google maps API, and does a bunch of logic before presenting the necessary
          informaton.
        </p>
        <a href="https://stream.cls.health/match" target="_blank" class="btn">
          Visit stream.cls.health
        </a>
      </div>
    </div>
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">Genshin Birthdays</h5>
        <p class="card-text">
          This one's a simple, single purpose project. In the game "Genshin Impact", characters have
          birthdays that give you rewards if you log in on that day. This site simply lets you know
          whose birthday it is today, and also has functionality to alert subscribers via webhooks,
          who are saved in a MongoDB cluster.
        </p>
        <a href="https://genshin-birthdays.com" target="_blank" class="btn">
          Visit genshin-birthdays.com
        </a>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card-container {
  display: flex;
  justify-content: space-around;
  flex-wrap: nowrap;
  gap: 2rem;
}

.card {
  width: 18rem;
}

.card .card-body {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
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
}
</style>
