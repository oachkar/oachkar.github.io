<template>
  <section id="sites">
    <h2>Websites</h2>
    <p>
      I also develop websites, including the one you're on right now. I like to keep things simple,
      lightweight, and easy to use. Though I am a sucker for the occasional flashy landing page with
      scroll animations... in moderation. Check some of them out.
    </p>
    <div class="card-container">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">CLS Stream</h5>
          <p class="card-text">
            A web application developed for the multi-speciality clinic CLS Health in Webster,
            Texas. Though it is an internal tool, here is one public facing application. It utilizes
            React and Bootstrap for the front end, and communication with a backend API that hits a
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
          <h5 class="card-title">CLS Health</h5>
          <p class="card-text">
            While stream.cls.health is an internal facing tool, cls.health is the patient facing
            page. I currently contribute to and help maintain this site, powered by Next.js,
            Tailwind, Prismic, and Vercel. I'm responsible for developing new features with a focus
            on UX and interactivity, and creating components that the internal content team can use
            to efficiently build and modify pages.
          </p>
          <a href="https://cls.health" target="_blank" class="btn"> Visit cls.health </a>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Genshin Birthdays</h5>
          <p class="card-text">
            This one's a simple, single purpose project. In the game "Genshin Impact", characters
            have birthdays that give you rewards if you log in on that day. This site simply lets
            you know whose birthday it is today, and also has functionality to alert subscribers via
            webhooks, who are saved in a MongoDB cluster.
          </p>
          <a href="https://genshin-birthdays.com" target="_blank" class="btn">
            Visit genshin-birthdays.com
          </a>
        </div>
      </div>
    </div>
  </section>
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
