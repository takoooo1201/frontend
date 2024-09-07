<template>
  <h1>HEllo Hello</h1>
  <roturer-link to="/upload">Upload</roturer-link>
  <roturer-link to="/chatbot">Chatbot</roturer-link>
  <roturer-link to="/autofillform">AutoFillForm</roturer-link>
  
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <div>
    <router-view />
  </div>  
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    //HelloWorld
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




