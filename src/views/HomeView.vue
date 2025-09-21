<template>
  <div>
    <img class="main-img" src="@/assets/img/bg.jpg" />
    <div class="box">
      <img class="box__img" src="@/assets/img/me-1.jpeg" />
      <div class="box__content">
        <h2>Meet Harry</h2>
        <p>Hello, I’m Harry, a professionally trained gardener with RHS Level 2 Horticulture and Garden Design qualifications from Plumpton College. My main focus is garden maintenance and care, ensuring outdoor spaces stay healthy, vibrant, and enjoyable all year round.</p>
        <p>I take an eco-friendly, wildlife-friendly approach, encouraging plant diversity and sustainable practices so gardens not only look their best but also support nature. From regular upkeep to seasonal care, I bring knowledge, reliability, and a passion for helping gardens thrive.</p>
      </div>
    </div>
    <div class="services">
      <p>Mowing </p>
      <p>Hedge cuttiner </p>
      <p>Pruning </p>
      <p>Planting trees and plants </p>
      <p>Creating beds </p>
      <p>Mulching </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
}
</script>

<style lang="scss">
body {
  margin: 0;
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
  max-width: 100%;
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

.box {
  margin: auto;
  position: relative;
  background-color: white;
  display: flex;

  @media screen and (min-width: 767px) {
    top: -200px;
    margin-bottom: -200px;
    width: 900px;
  }

  &__img {
    width: 50%;
    img {
      max-width: 100%;
    }
  }

  &__content {
    width: 50%;
    padding: 65px;
    padding-top:20px;

    h4 {
      text-align: center;
    }
  }
}
</style>
