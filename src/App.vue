<template>
  <div id="app">
    <nav>
      <div>
        <router-link class="bg-white" to="/">Home</router-link> |
        <router-link to="/about">About</router-link>
      </div>
      
    </nav>
    <router-view/>
    <!-- <home-view></home-view> -->
  </div>
</template>

<script>
// import HomeView from '@/views/HomeView.vue'

export default {
  name: 'MasterVue',
  components: {
    // HelloWorld
    // HomeView
  }
}
</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  /* color: #fff; */
}
/* 

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
} */
</style>
