<template>
    <nav>
    <router-link to="/" class="wording" >Home</router-link>

    </nav>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
nav {
    background-color: lightsalmon;
    padding: 2rem;
  }
  
  nav a {
    text-decoration: none;
  }
  
  nav a.router-link-exact-active {
    color: black;
  }
</style>