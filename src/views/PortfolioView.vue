<script setup>
import GameJamCards from '@/components/GameJamCards.vue'
import WebsitesCards from '@/components/WebsitesCards.vue'
import Profile from '@/components/ProfileCard.vue'
import { onMounted, onUpdated } from 'vue'

const observerOptions = {
  root: null,
  rootMargin: '0px',
  threshold: 0.05,
}

function observerCallback(entries) {
  console.log(entries)
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
    <section id="profile" class="c-invisible">
      <Profile />
    </section>
    <hr />
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
        skills to do it well alone. These projects are a testament to my ability to work in teams
        and communicate with artists, composers, and designers to work collaboratively towards a
        single vision, as well as my ability to realistically manage a project within a strict
        deadline.
      </p>
      <GameJamCards />
      <br />
    </section>
    <hr />

    <section id="sites" class="c-invisible">
      <h2>Websites</h2>
      <p>
        I also develop websites, including the one you're on right now. I like to keep things
        simple, lightweight, and easy to use. Though I am a sucker for the occasional flashy landing
        page with scroll animations... in moderation. Check some of them out.
      </p>
      <WebsitesCards />
    </section>
    <hr />

    <section id="about" class="c-invisible">
      <div>
        <h2>About Me</h2>
        <p>
          I'm a software, web, and game developer with a strong focus on user experience,
          optimization, and good internal design. <br />
        </p>
        <h4>Education</h4>
        <p>
          <b>Bachelor of Science</b> in Computer Science, with a Minor in Media Production, from the
          University of Houston. <br />
          <b>Master of Science</b> in Cybersecurity from the University of Houston. <br />
        </p>
        <h4>Skills</h4>
        <p>
          <b>Web Development:</b> I'm a professional web developer with experience serving and
          deploying websites using cloud services, configuring webservers like Apache/Nginx, and
          using Docker for application containerization. I also have extensive experience in backend
          environment development including developing web APIs, as well as configuring backend
          services such as SQL servers.
        </p>
        <p>
          <b>Game Development:</b> My game development proficencies are in systems design,
          programming, and mechanics implementation. I also enjoy UX/UI design and game design, and
          thoroughly enjoy working collaboratively with others in various disciplines to bring ideas
          to life.
        </p>
        <h4>Tools</h4>

        <b>Game Engines:</b> Godot, Unity
        <br />
        <b>Web Frameworks/Tools:</b> React, Vue, Node.js, Next.js, Flask, Django, Express
        <br />
        <b>Backend:</b> AWS, Digital Ocean, SQL Server, Postgres, Apache, Nginx, Docker
        <br />
        <b>Languages:</b> HTML, CSS, Python, JavaScript, C++, C#, Java, SQL
        <br />
        <b>OS:</b> Windows, Linux
        <br />
        <b>Software:</b> Git, Photoshop, Clip Studio Paint, Premiere Pro, Visual Studio Code
      </div>
    </section>
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
