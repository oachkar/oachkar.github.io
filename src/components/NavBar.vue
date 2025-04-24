<template>
  <nav class="g-navbar" ref="nav">
    <ul class="nav nav-pills">
      <li class="nav-item">
        <a href="#projects">Games</a>
      </li>
      <li class="nav-item">
        <a href="#sites">Websites</a>
      </li>
      <li class="nav-item">
        <a href="#about">About</a>
      </li>
      <li class="nav-item">
        <a href="#links">Links</a>
      </li>
      <li class="nav-item">
        <a href="#contact">Contact</a>
      </li>
    </ul>
  </nav>
</template>

<style scoped>
.g-navbar {
  background-color: rgb(32, 32, 32);
  box-shadow: #42b883 0 2px 0px;
  justify-content: center;
  position: fixed;
  width: 100%;
  left: 0;
  top: 0;
  z-index: 9999;
  margin-top: 0;
  padding: 0;
}

.g-navbar ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
}

.g-navbar ul li {
  display: inline;
  font-size: 1.5rem;
}

.g-navbar ul li a {
  display: block;
  padding: 14px 16px;
}
.g-navbar ul li a:active {
  background-color: #42b883;
}

@media (max-width: 800px) {
  .g-navbar ul li {
    display: inline;
    font-size: initial;
  }
  .g-navbar ul li a {
    padding: 14px 11px;
  }
}
</style>
