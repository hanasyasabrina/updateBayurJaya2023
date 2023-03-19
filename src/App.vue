<template>
  <div id="app" class="header w-full h-full">
    <div class="header__top h-full rounded-t-2xl w-full text-white flex flex-row px-6">
      <div class="flex justify-center py-4 font-bold">PT. Bayur Jaya</div>
      <div class="flex flex-row ml-auto py-4 gap-10">
        <div>info@bayurjaya.co.id</div>
        <div>+62 21 552 6610</div>
        <div>Tangerang</div>
        <div><router-link to="/contact">Contact</router-link></div>
      </div>
    </div>
    <div class="header__bottom rounded-t-2xl w-full px-6">
      <nav class="flex justify-center items-center flex-row py-6">
        <div class="header--logo"></div>
        <div class="flex h-12 ml-auto gap-8">
          <router-link to="/">Home</router-link>
          <router-link to="/expertise">Expertise</router-link>
          <router-link to="/gallery">Gallery</router-link>
          <router-link to="/about">Insider</router-link>
          <router-link to="/overons">Over ons</router-link>
        </div>
        
      </nav>
    </div>
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
  border-bottom: 4px solid #e33c38;
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
