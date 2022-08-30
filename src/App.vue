<template>
  <HomeView/>
</template>

<script>

import HomeView from './views/HomeView.vue';

export default {
  name: 'App',
  components: {
    HomeView
}
}
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300&family=Poppins&display=swap');

* {
  margin: 0;
  box-sizing: border-box;
}

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #0e1111;
}

h1, h3, h4 {
  font-family: 'Cormorant Garamond', serif;
}

h2, p {
  font-family: 'Poppins', sans-serif;
}

h2 {
  font-size: 1rem;
  margin-top: 1.8rem;
  text-transform: uppercase;
}

h3 {
  font-size: 1.9rem;
  margin: 0.6rem 0 0.6rem;
  text-transform: capitalize;
}

h4 {
  font-size: 1.4rem;
  margin: 1rem 0;
}

button {
    background-color: #3FA48C;
    border-radius: 8px;
    border: none;
    padding: 16px;
    color: #fff;
    box-shadow: 0px 2px 2px rgba(0, 0, 0, 0.25);
    margin-top: 8px;
}

</style>
