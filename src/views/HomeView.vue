<template>
  <NavBar/>
  <PageHeader/>
  <AboutMe/>
  <ToolBox/>
  <MyWork/>
  <ContactForm/>
  <PageFooter/>
</template>

<script>
import NavBar from './../components/NavBar.vue';
import PageHeader from './../components/PageHeader.vue';
import AboutMe from './../components/AboutMe.vue';
import ToolBox from './../components/ToolBox.vue';
import MyWork from './../components/MyWork.vue';
import ContactForm from './../components/ContactForm.vue';
import PageFooter from './../components/PageFooter.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    PageHeader,
    AboutMe,
    ToolBox,
    MyWork,
    ContactForm,
    PageFooter
}
}

</script>

<style>


</style>