<script setup>
import GameJamCards from '@/components/GameJamCards.vue'
import WebsitesCards from '@/components/WebsitesCards.vue'
import { onMounted } from 'vue'

const observerOptions = {
  root: null,
  rootMargin: '0px',
  threshold: 0.2,
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

onMounted(() => {
  const observer = new IntersectionObserver(observerCallback, observerOptions)
  const fadeElms = document.querySelectorAll('.c-invisible')
  fadeElms.forEach((el) => observer.observe(el))
})
</script>

<template>
  <main>
    <section id="projects" class="c-invisible">
      <h2>Game Jam Projects</h2>
      <p>
        I've been involved in a number of game jams in which I worked very closely with team members
        to produce a fully featured demo within a short time. My responsibilities and contributions
        consisted of the programming and implementation of game mechanics. The art in Pepper Hermit
        was mostly made by me.
        <br />
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
        <h5>Omar Achkar</h5>
        <p>
          Software, web, and game developer with a passion for user experience and good internal
          design. <br />
        </p>
        <h4>Education</h4>
        <p>
          <b>Bachelor of Science</b> in Computer Science, with a Minor in Media Production, from the
          University of Houston. <br />
          <b>Master of Science</b> in Cybersecurity from the University of Houston. <br />
        </p>
        <h4>Skills</h4>
        <p>
          <b>Web Development:</b> Proficient in HTML, CSS, JavaScript, and frameworks such as Vue
          and React. Experienced with tools such as Node.js and source control using Git. I have
          professional experience serving and deploying websites using cloud services such as AWS
          and Digital Ocean, configuring webservers like Apache/Nginx, using Docker for application
          containerization, and managing DNS. I also have extensive experience in backend
          environment development including developing web APIs such as with Flask or Django, as
          well as configuring backend services such as SQL servers.
          <br />
          <b>Game Development:</b> I am proficient in the Godot game engine with equal experience in
          the Unity game engine. I can work comfortably in C# and C++ in these environments. My
          expertise in game development is in the programming and software design side of things, as
          I enjoy building elegant solutions with a focus on user experience being as simple as
          possible. I enjoy documentation and working in teams, and always strive to make my fellow
          developers' lives easier.
          <br />
          <b>Languages:</b> Python, JavaScript, C++, C#, Java
          <br />
          <b>OS:</b> Windows, Linux
          <br />
          <b>Software:</b> Photoshop, Clip Studio Paint, Premiere Pro, Visual Studio Code
        </p>
      </div>
    </section>
    <hr />

    <section id="links" class="c-invisible">
      <h2>Links</h2>
      <p>
        <a href="https://github.com/fresh4">GitHub</a> •
        <a href="https://fresh4.itch.io/">Itch</a> •
        <a href="https://www.linkedin.com/in/omar-achkar/">LinkedIn</a>
      </p>
    </section>
    <hr />

    <section id="contact" class="c-invisible">
      <h2>Contact Me</h2>
      <p>
        For professional inquiries, contact me at
        <a href="mailto:omar.achkar98@gmail.com"> omar.achkar98@gmail.com </a> <br />

        For academic inquiries, contact me at
        <a href="mailto:oachkar@uh.edu"> oachkar@uh.edu </a> <br />
      </p>
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
