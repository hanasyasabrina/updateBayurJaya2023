<template>
  <div id="app" class="header w-full h-full">
    <div id="nav" class="w-full h-full">
      <div class="header__top h-full rounded-t-2xl w-full text-white flex flex-row px-6 items-center">
        <div class="flex justify-center py-4 font-bold">PT. Bayur Jaya</div>
        <div class="flex flex-col xl:flex-row ml-auto py-4 gap-1 xl:gap-10 text-sm xl:text-base">
          <div class="hide-mobile"><a href="mailto:info@bayurjaya.co.id?subject=Mail from Our Site">info@bayurjaya.com</a></div>
          <div class="hide-mobile"><a href="tel:0215526610">Call +62 21 552 6610</a></div>
          <div class="hide-mobile">Tangerang</div>
          <div><router-link to="/contact">Contact</router-link></div>
        </div>
      </div>
      <div class="header__bottom w-full px-6 transition-all" :class="[active? 'fixed top-0 left-0 rounded-none z-[12] duration-100' : 'relative rounded-t-2xl duration-150']">
        <nav class="flex justify-center items-center flex-row" :class="[active? 'py-4' : 'py-6']">
          <div class="header--logo" ></div>
          <div class="flex h-20 xl:h-12 xl:ml-auto gap-8 menu-scroll-mobile text-base xl:text-xl items-center">
            <router-link class="p-1" to="/">Home</router-link>
            <router-link class="p-1" to="/expertise">Expertise</router-link>
            <router-link class="p-1" to="/gallery">Gallery</router-link>
            <router-link class="p-1" to="/about">About</router-link>
            <!-- <router-link class="p-1" to="/overons">Over ons</router-link> -->
          </div>
        </nav>
      </div>
    </div>
    
    <router-view/>
    <footer-view/>
  </div>
</template>

<script>
import FooterView from '@/views/FooterView.vue'

export default {
  name: 'MasterVue',
  components: {
    FooterView
  },
  data(){
    return{
      active: false,
    }
  },
  methods:{
  },
  mounted(){
    window.document.onscroll = () => {
      let navBar = document.getElementById('nav');
      if(window.scrollY > navBar.offsetTop){ 
        this.active = true;
        } else {
        this.active = false;
      }
    }
  }
}
</script>


<style lang="scss" scoped>
   @mixin smartphone {
    @media (max-width: 599px) { @content; }
  }
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #0A2753;
}
.header{

  &__top{
    background-color: #0A2753;
  }
  &__bottom{
    background-color: white;
    font-family: 'Montserrat';
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
  @include smartphone{
    border-bottom: 2px solid #e33c38;
  }
}

.hide-mobile{
  display: flex;
  @include smartphone{
    display: none !important;
  }
}
.menu-scroll-mobile{
  @include smartphone{
    overflow-x: scroll;
    margin-left: 25px;
    max-width: 280px;
  }
}

.menu-scroll-mobile::-webkit-scrollbar-track
{
  border-radius: 10px;
  background-color: #f3f3f3;
}

.menu-scroll-mobile::-webkit-scrollbar
{
	height: 4px;
}

.menu-scroll-mobile::-webkit-scrollbar-thumb
{
	border-radius: 10px;
	-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,.3);
	background-color: #0e1c4b;
}

</style>
