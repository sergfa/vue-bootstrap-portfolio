<template>
  <div id="app">
    <app-nav-bar></app-nav-bar>
    <app-banner></app-banner>
    <app-qualities></app-qualities>
    <app-contact></app-contact>
    <app-projects></app-projects>
    <app-social></app-social>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Banner from './components/Banner.vue'
import Qualities from './components/Qualities.vue'
import Contact from './components/Contact.vue'
import Projects from './components/Projects.vue'
import Social from './components/Social.vue'
import Footer from './components/Footer.vue'
import NavBar from './components/Navbar.vue'


export default {
  name: 'App',
  components: {
    appBanner: Banner,
    appQualities: Qualities,
    appContact: Contact,
    appProjects: Projects,
    appSocial: Social,
    appFooter: Footer,
    appNavBar: NavBar
  }
}
</script>

<style lang="scss">
  @import './styles/custom_bootstrap.scss';
  @import '../node_modules/bootstrap/scss/bootstrap.scss';
</style>

<style>
body {
  margin-top: 60px;
}
h1, h2, h3, h4, h5 {
  font-family: 'Roboto Condensed', sans-serif;
}

.height-100 {
  min-height: 100vh;
}
.height-80 {
  min-height: 80vh;
}
.height-60 {
  min-height: 60vh;
}
.height-50 {
  min-height: 50vh;
}
.height-40 {
  min-height: 40vh;
}

#banner,
#contact,
#social {
  background: linear-gradient(rgba(129, 69, 19, 0.6), rgba(129, 69, 19, 0.6)), url('./assets/img/portret.jpg');
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
}
</style>