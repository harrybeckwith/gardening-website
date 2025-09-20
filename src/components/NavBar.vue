<template>
  <div class="container">
   <div class="navbar">
    <div class="navbar__container">
      <img class="navbar__container__logo" src="../assets/icons/logo.png"/>
      <h5 class="navbar__container__name"><a href="#"> Harry Beckwith Gardens</a></h5>
    </div>
        <nav>
          <ul>
            <li><a href="tel:07446738376"><button> <img class="phone-icon" src="../assets/icons/phone.svg"/> <p>07446 738 376</p></button></a></li>
            <li><a href="#"><button>Book</button></a></li>
          </ul>
        </nav>
      </div>
      </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

a:visited {
  color: inherit;
}

button {
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
  height: 40px;
  font-size: 14px;
  font-weight: 500;
  padding:10px;
  width: 157px;
  border: none;
  border-radius: 5px;
  transition: all 0.5s ease-in-out;
  background-color: #006e48;
  color: white;

  &:hover {

    opacity: 0.3;
  }
}
.phone-icon {
  width: 20px;
  margin-right: 10px;
}
.container {

  border-bottom: 1px solid rgb(214, 214, 214);
}
.navbar {
  display: flex;
  width: 80%;
  margin: auto;
  align-items: center;
  justify-content: space-between;
  height: 100%;

  &__container {
    display:flex; 
    align-items: center;

    &__name {
      color: black;
    }

    &__logo {
      width: 80px;
    }
  }
  
 


  ul {
    display: flex;

      li {
        list-style-type: none;
        padding: 10px;
        margin: 0 10px;

        a {
          color: red;
            &:hover {
              color: var(--secondary-color);
            } 
        }
      }
  }
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
