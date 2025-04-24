<script setup>
import GameJamCards from '@/components/GameJamCards.vue'
</script>

<template>
  <main>
    <section id="projects" ref="projects">
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

    <section id="about" ref="about">
      <div>
        <h2>About Me</h2>
        <h5>Omar Achkar</h5>
        <p>
          Software, web, and game developer with a passion for user experience and good internal
          design. <br />
        </p>
        <h4>Education</h4>
        <p>
          <b>Bachelor of Science</b> in Computer Science from the University of Houston. <br />
          <b>Master of Science</b> in Cybersecurity from the University of Houston. <br />
        </p>
        <h4>Skills</h4>
        <p>
          <b>Web Development:</b> Proficient in HTML, CSS, JavaScript, and frameworks such as Vue
          and React. Experienced with tools such as Node.js. I have professional experience serving
          and deploying websites using cloud services such as AWS and Digital Ocean, and configuring
          webservers like Apache/Nginx, using Docker for application containerization, and managing
          DNS. I also have extensive experience in backend environment development including
          developing web APIs such as with Flask or Django, as well as configuring backend services
          such as SQL servers.
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

    <section id="links" ref="links">
      <h2>Links</h2>
      <p>
        <a href="https://github.com/fresh4">GitHub</a> •
        <a href="https://fresh4.itch.io/">Itch</a> •
        <a href="https://www.linkedin.com/in/omar-achkar/">LinkedIn</a>
      </p>
    </section>
    <hr />

    <section id="contact" ref="contact">
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
  background-color: rgb(32, 32, 32);
  border-radius: 0.5rem;
  border: 2px black;
  padding: 1rem;
  padding-bottom: 1rem;
}
</style>
