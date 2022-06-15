<template>
<div id="nav">
  <navbar/>
  </div>
  <router-view/>
</template>
<script>
import Navbar from '../src/components/Navbar.vue'
export default{
  components:{
    Navbar
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

#nav {
  padding: 30px;
  text-align: center;
}

/* #nav a {
  font-weight: bold;
  color: #2c3e50;
    font-size: 3rem;
  text-decoration: none;
  padding: 2rem;
}

#nav a.router-link-exact-active {
  color: #42b983;
} */
</style>
