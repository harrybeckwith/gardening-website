<template>
  <div id="app">
    <div class="container">
      <NavBar/>
    </div>
  <router-view></router-view>

  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'

export default {
  name: 'App',
  components: {
    NavBar
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,100;0,300;0,400;0,700;0,900;1,100;1,300;1,400;1,700;1,900&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
body {
  margin: 0;
  background-color: #FAF9F6;
  font-family: "Poppins", sans-serif;
  font-weight: 400;
  font-style: normal;
  color: #444444;
}

p {
    font-size: 15px;
}

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

a,
a:link,
a:visited,
a:hover,
a:active {
  color: black; /* Or any color, like #333, inherit, etc. */
  text-decoration: none; /* Removes the underline */
}

.main-img {
  max-height: 100vh;
width: 100%;
}

.container {
  background-color: var(--nav-color);
  height: 70px;
}







@media screen and (min-width: 390px) and (max-width: 767px) {
  .container {
    height: 100%;
  }
  .container .navbar {
    flex-direction: column;
  }
}
</style>
