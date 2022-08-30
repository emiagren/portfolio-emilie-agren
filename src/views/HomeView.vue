<template>
  <NavBar/>
  <PortfolioTop/>
  <AboutMe/>
  <ToolBox/>
  <MyWork/>
  <ContactForm/>
</template>

<script>
import NavBar from './../components/NavBar.vue';
import PortfolioTop from './../components/PortfolioTop.vue';
import AboutMe from './../components/AboutMe.vue';
import ToolBox from './../components/ToolBox.vue';
import MyWork from './../components/MyWork.vue';
import ContactForm from './../components/ContactForm.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    PortfolioTop,
    AboutMe,
    ToolBox,
    MyWork,
    ContactForm
}
}

</script>

<style>


</style>