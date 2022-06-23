<template>
  <nav>
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
    <router-link to="/services">Services</router-link>
    <router-link to="/projects">Projects</router-link>
    <router-link to="/news">News</router-link>
    <router-link to="/contact">Contact</router-link>
  </nav>
  <router-view />
  <Footer />
</template>

<script>
import Footer from '@/components/Footer';

export default {
  name: 'App',
  components: {
    Footer
  }
}
</script>

<style>
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #e3e3e3;
  background: #27282e;
}

nav {
  width: 100vw;
  padding: 30px;
  background: transparent;
}

nav a {
  font-weight: bold;
  color: #e6e6e6;
  text-decoration: none;
  margin-right: 3rem;
}

nav a.router-link-exact-active {
  color: #0083cf;
}
</style>
