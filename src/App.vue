<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HomePage msgss="my home"/>
  <HelloWorld></HelloWorld>
  <ContactPage></ContactPage>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import HomePage from './components/Home.vue'
import ContactPage from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    HomePage,
    ContactPage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
