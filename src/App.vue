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

@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond&family=La+Belle+Aurore&family=Poppins&display=swap');
* {
  margin: 0;
  box-sizing: border-box;
}

.wrapper {
  max-width: 1280px;
  margin: 0 auto;
  padding: 0 8%;
}

h1, h2, p {
  font-family: 'Poppins', sans-serif;
  color: #343434;
}

h3, h4 {
  font-family: 'Cormorant Garamond', serif;
  text-shadow: rgb(116, 116, 116);
}

h2 {
  font-size: 1rem;
  margin: 2rem 0 0.6rem;
  text-transform: uppercase;
}

h3 {
  color: #fff;
  font-size: 2rem;
  text-transform: capitalize;
  margin: 0 0 1rem;
}

h4 {
  font-size: 1.4rem;
  margin: 2rem 0 1rem;
}

p {
  line-height: 1.55;
  font-size: 1rem;
  margin: 0 0 1rem;
}

button {
  background-color: #3FA48C;
  border-radius: 8px;
  border: none;
  padding: 1rem;
  margin: 0.6rem 0.6rem 0.6rem 0;
  font-size: 1.1rem;
  color: #fff;
  box-shadow: 0px 2px 2px rgba(0, 0, 0, 0.25);
  cursor: pointer;
}

a {
  color: #fff;
  text-decoration: none;
  font-size: 1.1rem;
  cursor: pointer;
}

.icon {
    padding: 0 0.8rem;
    text-align: center;
}

.icons-wrapper {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin: 0 0 1.6rem;
}

</style>
