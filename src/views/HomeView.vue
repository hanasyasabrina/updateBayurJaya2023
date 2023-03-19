<template>
  <div class="home relative w-full">
    <div class="flex flex-col justify-center items-center w-full mb-14 homee--catalog">
          <div class="font mb-8 text-5xl max-w-5xl h-16 not-italic font-bold">Build On Safety Is Our Foundation</div>
          <div class="font-isi absolute max-w-screen-lg h-14 left-64 right-64 not-italic font-normal text-base top-14 text-center">Kami adalah spesialis Jasa Konstruksi, Pengadaan Barang & Jasa dan Perdagangan Umum untuk pekerjaan dalam bidang Mekanikal & Elektrikal, Sipil, Telematika dan Jasa lainnya. Kami bangga dapat memberikan kualitas dan solusi luar biasa untuk klien terkemuka di seluruh Indonesia.</div>
    </div>
    <!-- start swiper -->
    <div class="swiper">
      <div class="swiper-wrapper">
        <!-- Slides -->
        <div class="swiper-slide" v-for="(index, key) in dataFoto" :key="key">
            <img :src="require(`../assets/homeAssets/${index.url}`)"/>
        </div>
      </div>
      <!-- If we need pagination -->
      <div class="swiper-pagination"></div>
    </div>
    <!-- end swiper -->

    <div @click="testClick" class="items-center justify-center">
      <button class="homee--download items-center justify-center">DOWNLOAD COMPANY PROFILE</button>
    </div>

    <div class="ml-96 pl-46 mr-96 my-8 border-solid border border-blue-900 place-items-right">

    </div>

    <div class="max-w-screen-md w-fit lg:max-w-screen-md lg:flex my-8 place-items-center mx-80">
    <div class="col-span-1 flex-none bg-cover object-contain rounded-xl rounded-t-xl rounded-b-xl h-72 w-48 overflow-hidden place-items-center">
      <img :src="require('../assets/owner-min.png')">
      </div>
    <div class="bg-white rounded-b lg:rounded-b-none lg:rounded-r p-4 flex flex-col place-items-center leading-normal">
        <div class="mb-8 ml-3">
          <div class="font text-gray-900 font-bold text-6xl mb-2 text-left">Sungkono</div>
            <p class="font font-bold text-gray-400 text-left text-2xl">Owner</p>
            <p class="border-solid border border-blue-900"></p>
            <p class="text-gray-700 text-base text-left">Kami berkomitmen untuk memberikan yang terbaik kepada anda dengan memperhatikan keselamatan, kualitas dan kepuasan dengan terus memperbarui sistem kami untuk memastikan project berjalan lancar dan efisien.</p>
        </div>
      </div>
      </div>
    
    <div class="imgPartners flex flex-col justify-center items-center w-full mb-14">
          <div class="mb-8 text-3xl">CLIENTS & PARTNERS</div>
    <!-- start swiper -->
    <div class="swiper swiper-partners">
      <div class="swiper-wrapper">
        <div class="swiper-slide" v-for="(index, key) in dataPartners" :key="key">
          <img :src="require(`../assets/partners/${index.url}`)"/>
        </div>
      </div>         
    </div>
    <div class="w-full h-full relative">
      <div class="swiper-button-prev swiper-button-prev-partners"></div>
        <div class="swiper-button-next swiper-button-next-partners"></div>
    </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

// import { container } from 'webpack';

export default {
  name: 'HomeView',
  components: {
   // container
},
  data(){
    return{
      swiperTest: null,
      dataFoto:[
        {
          url:"CCTV.png",
          tag: "cctv",
        },
        {
          url:"HDD BORING.png",
          tag: "boring",
        },
        {
          url:"MECHANICAL & ELECTRICAL.png",
          tag: "mekanikal",
        },
        {
          url:"SIPIL.png",
          tag: "sipil",
        }
      ],

      swiperPartners: null,
      dataPartners:[
        {
          url:"partners-1.png",
          tag:"partners",
        },
        {
          url:"partners-2.png",
          tag:"partners",
        },
        {
          url:"partners-3.png",
          tag:"partners",
        },
        {
          url:"partners-4.png",
          tag:"partners",
        },
        {
          url:"partners-5.png",
          tag:"partners",
        },
        {
          url:"partners-6.png",
          tag:"partners",
        },
        {
          url:"partners-7.png",
          tag:"partners",
        },
        {
          url:"partners-8.png",
          tag:"partners",
        },
        {
          url:"partners-9.png",
          tag:"partners",
        },
        {
          url:"partners-10.png",
          tag:"partners",
        },
        {
          url:"partners-11.png",
          tag:"partners",
        },
        {
          url:"partners-12.png",
          tag:"partners",
        },
        {
          url:"partners-13.png",
          tag:"partners",
        },
        {
          url:"partners-14.png",
          tag:"partners",
        },
        {
          url:"partners-15.png",
          tag:"partners",
        },
        {
          url:"partners-16.png",
          tag:"partners",
        },
        {
          url:"partners-17.png",
          tag:"partners",
        },
        {
          url:"partners-18.png",
          tag:"partners",
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
    },

    initSwiperPartners(){
      // eslint-disable-next-line
        this.swiperPartners = new Swiper('.swiper-partners', {
          spaceBetween: 30,
          autoHeight: false,
          centeredSlides: true,
          loop: true,
          slidesPerView: 3,
          navigation: {
            nextEl: ".swiper-button-next-cctv-tes",
            prevEl: ".swiper-button-prev-cctv-tes"
          }
        });
      },
  },
  mounted(){
    this.initSwiperTest()
    console.log(this.dataFoto)
    this.initSwiperPartners()
    console.log(this.dataPartners)
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
		background:white;
		border-radius: 6px;
		transition: all .5s ease-in-out;
		transform: scale(.8);

    &.swiper-slide-active {
      background: white;
      opacity:1;
      transform: scale(1);
      z-index: 3;
    }

		
}

.swiper-button-next,.swiper-button-prev{
    top: -100px;
  }
  .swiper-button-next{
    // position: relative;
    right: -15px;
    // top: 20%;
    &::after{
      content: "";
      background-image: url('../assets/ornament/btn-next.png');
      padding: 100%;
      background-size: contain;
      background-repeat: no-repeat;
      background-position: center;
      
    }
  }
  .swiper-button-prev{
    // position: relative;
    left: -15px;
    // left: 150px;
    // top: 20%;
    &::after{
      content: "";
      background-image: url('../assets/ornament/btn-prev.png');
      padding: 100%;
      background-size: contain;
      background-repeat: no-repeat;
      background-position: center;
    }
  }

.swiper-slide-2 {
		margin: 32px 0;
		height: auto;
		width: 100%;
		padding: 0;
		opacity: .8;
		background:white;
		border-radius: 6px;
		transition: all .5s ease-in-out;
		transform: scale(.8);

    &.swiper-slide-active-2 {
      background:white;
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

.imgPartners{
  margin-top: -1px;
    background-color: white;
}

.font{
  font-family: 'Montserrat';
}

.font-isi{
  font-family: 'Cabin';
}

.homee{
  font-family: 'Montserrat, Inter';
    background-color: white;
    margin-top: -1px;

    &--download{
      padding: 20px 64px;
      background-color: #0E1C4B;
      transition: 0.5s;
      color: white;
      font-family: 'Inter';
      font-weight: 700;
      font-size: 18px;
      border-radius: 4px;
      // max-width: 165px;
      cursor: pointer;
      &:hover{
        background-color: #4B0E0E;
      }
    }

    &--catalog{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: 200px;
      left: -520px;
      background-image: url('../assets/ornament/insider6.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 50px;
      height: 350px;
      }
    }

    &--catalog2{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: 200px;
      left: -520px;
      background-image: url('../assets/ornament/insider5.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 50px;
      height: 350px;
      }
    }
}




</style>
