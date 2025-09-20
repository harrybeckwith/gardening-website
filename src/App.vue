<template>
  <div id="app">
    <div class="container">
      <NavBar/>
        <iframe src="https://docs.google.com/forms/d/e/1FAIpQLScaM-_vj1Al64B4rcNFvpcIgPqbRV-pJ9km1plOicFVjcU2pg/viewform?embedded=true" width="640" height="959" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
    </div>
    <!-- <img class="main-img" src="./assets/logo.png" > -->
     <img class="main-img" src="./assets/icons/bg.jpg"/>
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
body {
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
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
