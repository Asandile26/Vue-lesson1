<template>
 

<Navbar/>  
<router-view/>
<Footer/>
</template>
<script>
import Navbar from './components/navbar.vue';
import Footer from './components/footer.vue';


export default {
components:{
    Navbar,
    Footer
} 

}
</script>
<style>
|*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
html{
  width: 100vw;
  height: 100vh;
}
body{
  width: 100vw;
  height: 100vh;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
footer{
  position: fixed;
  bottom: 0;
}
</style>
