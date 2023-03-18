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
    <footer-view/>
  </div>
</template>

<script>
// import HomeView from '@/views/HomeView.vue'
import FooterView from '@/views/FooterView.vue'

export default {
  name: 'MasterVue',
  components: {
    // HelloWorld
    // HomeView
    FooterView
  },
  data(){
    return{

    }
  },
  methods:{
  }
}
</script>


<style lang="scss" scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  /* color: #fff; */
  background-color: #0A2753;
}
.header{
  // background-color: #0A2753;

  &__top{
    background-color: #0A2753;
  }
  &__bottom{
    background-color: white;
    font-family: 'Montserrat';
    font-size: 24px;
  }

  &--logo{
    background-image: url('./assets/logo-home.png');
    background-repeat: no-repeat;
    background-position: center;
    background-size: contain;
    width: 80px;
    height: 80px;
  }
}
.router-link-exact-active{
  border-bottom: 2px solid red;
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
