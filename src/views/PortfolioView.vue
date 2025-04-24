<script setup>
import GameJamCards from '../components/GameJamCards.vue'
</script>

<template>
  <!-- <header>
    <nav>
      <router-link to="/">Home</router-link>
      <router-link to="/portfolio">Portfolio</router-link>
      <router-link to="/about">About</router-link>
      <router-link to="/contact">Contact</router-link>
    </nav>
  </header> -->
  <main>
    <section class="projects">
      <h2>Game Jam Projects</h2>
      <p>
        I've been involved in a number of game jams in which I worked very closely with team members
        to produce a fully featured demo within a short time. My responsibilities and contributions
        consisted of the programming and and implementation of game mechanics. The art in Pepper
        Hermit was mostly made by me.
      </p>
      <GameJamCards />
    </section>

    <section class="about">
      <div>
        <h2>About Me</h2>
        <p>
          Software, web, and game developer with a passion for user experience and good internal
          design. <br />
        </p>
        <h4>Education</h4>
        <p>
          Bachelor of Science in Computer Science from the University of Houston. <br />
          Master of Science in Cybersecurity from the University of Houston. <br />
        </p>
        <h4>Skills</h4>
        <p>
          Web: HTML, CSS, JavaScript, Vue.js, React.js, Node.js, Python, SQL <br />
          Game: Godot, Unity, C#, C++ <br />
        </p>
      </div>
    </section>

    <section>
      <h2>Links</h2>
      <p>
        <a href="https://github.com/fresh4">GitHub</a> •
        <a href="https://fresh4.itch.io/">Itch</a> •
        <a href="https://www.linkedin.com/in/omar-achkar/">LinkedIn</a>
      </p>
    </section>

    <section class="contact">
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
}
</style>
