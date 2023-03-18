<template>
  <div id="app">
    <nav class="bg-blue-900 py-4 px-0 grid grid-cols-2 m-0">
      <div class="font text-left text-white pl-3.5">PT. Bayur Jaya</div>
      <div class="font text-right text-white pr-6 grid grid-cols-4">
        <div>
          <router-link to="/">info@bayurjaya.co.id</router-link>
        </div>
        <div>
          <router-link to="/">+62 21 552 6610</router-link>
        </div>
        <div>
          <router-link to="/">Tangerang</router-link>
        </div>
        <div>
          <router-link to="/">Contact</router-link>
        </div>  
        
      </div>
    </nav>
    <nav class="grid grid-cols-2 pl-3.5 rounded-t-xl bg-blend-lighten hover:bg-blend-darken">
      <div>
        <img alt="vue logo" src="./assets/Logo-min.png"> <v-spacer />
      </div>
      <div class="font text-right text-2xl self-center mr-7 grid grid-cols-6">
        <div>
          <router-link class="bg-white" to="/">Home</router-link>
        </div>
        <div>
          <router-link to="/expertise">Expertise</router-link>
        </div>   
        <div>
          <router-link to="/gallery">Gallery</router-link>
        </div>   
        <div>
          <router-link to="/insider">Insider</router-link>
        </div>
        <div>
          <router-link to="/overOns">Over Ons</router-link>
        </div>
        <div>
          <router-link to="/contact">Contact</router-link>
        </div>  
        
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
.holo{
  background-color: rgb(10,39,83);
  overflow: hidden;
  padding: 0;
}

.font{
  font-family: 'Montserrat';

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
