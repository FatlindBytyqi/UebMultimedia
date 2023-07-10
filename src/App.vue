<template>
  <div id="app">
    <HeaderComponent/>
    <router-view />
    <FooterComponent/>
</div>
</template>

<style>
#app {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
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
  text-decoration: none;
  font-size: 22px;
  margin-left:20px ;
}

nav a.router-link-exact-active {
  color: #4a67e9;
}

</style>

<script>
import HeaderComponent from './components//Header/HeaderComponent.vue';
import FooterComponent from './components/Footer/FooterComponent.vue';
export default {
  components: {
    HeaderComponent,
    FooterComponent
  }
}
</script>