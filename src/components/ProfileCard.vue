<template>
  <div class="profile">
    <img src="@/content/pfp-cropped.png" class="pfp" />
    <div>
      <h2>Omar Achkar</h2>
      <p>Software, Web, and Game Developer bringing ideas to life in Houston, Texas.</p>
      <h4>Links</h4>
      <p>
        <a target="_blank" href="https://github.com/fresh4">GitHub</a> •
        <a target="_blank" href="https://fresh4.itch.io/">Itch</a> •
        <a target="_blank" href="https://www.linkedin.com/in/omar-achkar/">LinkedIn</a>
      </p>
      <h4>Contact</h4>
      <p>
        For professional inquiries, contact me at
        <a href="mailto:omar.achkar98@gmail.com"> omar.achkar98@gmail.com </a> <br />

        For academic inquiries, contact me at
        <a href="mailto:oachkar@uh.edu"> oachkar@uh.edu </a> <br />
      </p>
    </div>
  </div>
</template>

<style scoped>
.profile img {
  margin-right: 2rem;
}
.profile {
  display: flex;
}
.pfp {
  width: 15rem;
  object-fit: cover;
  border-radius: 1rem;
}

@media (max-width: 600px) {
  .profile {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .profile img {
    margin-bottom: 2rem;
    margin-right: 0rem;
  }
}
</style>
