<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Footer from './components/Footer.vue'
</script>

<template>
  <body>
    <header>

<div class="Navigation">
  <nav>
    <ul class="menu">

      <router-link to="/">          
        <div class="logo">
          <img class="logotete" src="./assets/icons8-visage-100.png" alt="">
        </div>
      </router-link>


      <li><router-link to="/">Acceuil</router-link></li>
      <li><router-link to="/about">A propos</router-link></li>
      <li><router-link to="/contact">Contact</router-link></li>
      <li><router-link to="/projets">Projets</router-link></li>
      <li><router-link to="/test">test 404</router-link></li>
    </ul>
  </nav>
</div>




</header>

<main>
<RouterView />
</main>

<footer>
<Footer />
</footer>


  </body>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Varela+Round");




.logo img {
    width: 100px;
}
nav {
  background-color: #555;
}

nav ul {
  list-style: none;
  text-align: center;
}
nav ul li {
  display: inline-block;
}
nav ul li a {
  display: block;
  padding: 15px;
  text-decoration: none;
  color: wheat;
  font-weight: 800;
  text-transform: uppercase;
  margin: 0 50px;
}
nav ul li a,
nav ul li a:after,
nav ul li a:before {
  transition: all .5s;
}
nav ul li a:hover {
  color: black;
}

</style>
