<template>
  <section id="sites">
    <h2>Websites</h2>
    <p>
      I also develop websites, including the one you're on right now. I like to keep things simple,
      lightweight, and easy to use. If you're interested in a custom website, check out my
      <a href="https://template.oachkar.com" target="_blank">example landing page</a> for more
      information. I like to work with small or local business owners to kickstart their online
      presence, but I am open to (and have) worked with medium-to-large sized companies as a
      contractor to help with existing projects or as a consultant.
    </p>
    <div class="card-container">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Landing Page Template</h5>
          <p class="card-text">
            Interested in a custom website? This example landing page is the perfect representation
            of what I can make for you or your business quickly and affordably. <br />
            It is built with Astro for blazing fast delivery, Tailwind, and DaisyUI.
          </p>
          <a href="https://template.oachkar.com" target="_blank" class="btn">
            Visit template.oachkar.com
          </a>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">CLS Health</h5>
          <p class="card-text">
            cls.health is the patient facing page for CLS Health, a multispecialty clinic in
            Webster, Texas. I currently maintain this site, powered by Next.js, Tailwind, Prismic,
            and Vercel. I'm responsible for developing new features with a focus on UX and
            interactivity, and creating components that the internal content team can use to
            efficiently build and modify pages.
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
