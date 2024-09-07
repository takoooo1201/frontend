<template>
  <h1>Hello Hello</h1>
  <nav>
    <router-link to="/upload">Upload</router-link>
    <router-link to="/">Chatbot</router-link>
    <router-link to="/download?formname=travelform&userid=5&extra1=哈囉囉囉囉">Download</router-link>
  </nav>
  <!-- direct to download-->
  
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
