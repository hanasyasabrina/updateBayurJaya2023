<template>
  <div class="home relative w-full">
    <!-- start swiper -->
    <div class="swiper">
      <div class="swiper-wrapper">
        <!-- Slides -->
        <div class="swiper-slide" v-for="(index, key) in dataFoto" :key="key">
          SLIDE 1
            <img :src="require(`../assets/mekanikElektrikal/${index.url}`)"/>
        </div>
      </div>

      <!-- If we need pagination -->
      <div class="swiper-pagination"></div>
    </div>
    <!-- end swiper -->

    <div @click="testClick">CLICK ME</div>
    <div>test</div>
    
    <!-- <div @click="testClick" v-for="(key, index) in dataFoto" :key="key">{{ index.url }}</div> -->
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    // HelloWorld
  },
  data(){
    return{
      swiperTest: null,
      dataFoto:[
        {
          url:"tes1.png",
          tag: "mekanikal",
        },
        {
          url:"tes1.png",
          tag: "sipil",
        }
      ]
    }
  },
  methods:{
    initSwiperTest(){
      // eslint-disable-next-line
        this.swiperTest = new Swiper('.swiper', {
        loop: false,
        spaceBetween: -60,
        autoHeight: false,
        centeredSlides: true,
        slidesPerView: 3,
        autoplay:{
          delay: 2000
        },
        // If we need pagination
        pagination: {
          el: '.swiper-pagination',
        },

      });
    },
    testClick(){
      alert('INI HASIL @ KLIK METHOD')
    }
  },
  mounted(){
    this.initSwiperTest()
    console.log(this.dataFoto)
    // this.initSwiperRunway()
  }
}
</script>

<!-- vue, tailwind, sass, swiper -->

<style lang="scss" scoped>
.home{
  background: white;
  margin-top: -1px;

}
.swiper{
  background-color: #ffffff;
  width: 100%;
  height: 100%;
  
}
.swiper-slide {
		margin: 32px 0;
		height: auto;
		width: 100%;
		padding: 0;
		opacity: .8;
		background:lightgrey;
		border-radius: 6px;
		transition: all .5s ease-in-out;
		transform: scale(.8);

    &.swiper-slide-active {
      background:gray;
      opacity:1;
      transform: scale(1);
      z-index: 3;
    }

		
}


img{
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}



</style>
