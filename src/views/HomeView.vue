<template>
  <div class="home relative w-full">
    <div class="home--catalog flex flex-col justify-center items-center w-full mb-14">
          <div class="home--title mb-8 text-5xl max-w-5xl not-italic font-bold">Build On Safety Is Our Foundation</div>
          <div class="home--title_isi w-full flex max-w-screen-lg font-normal text-base text-center"><p>Kami adalah spesialis Jasa Konstruksi, Pengadaan Barang & Jasa dan Perdagangan Umum untuk pekerjaan dalam bidang Mekanikal & Elektrikal, Sipil, Telematika dan Jasa lainnya. Kami bangga dapat memberikan kualitas dan solusi luar biasa untuk klien terkemuka di seluruh Indonesia.</p></div>
    </div>
    <!-- start swiper -->
    <div class="swiper swiper-home">
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

    <div @click="testClick" class="flex justify-center items-center flex-col mt-8">
          <div class="home--download">DOWNLOAD COMPANY PROFILE</div>
        </div>
    <div class="home--catalog3 relative w-full">
      <div class="max-w-screen-md w-fit lg:max-w-screen-md lg:flex my-10 place-items-center ml-56 mr-40 py-7 inset-y-56">
      <div class="img--owner col-span-1 flex-none bg-cover object-contain rounded-xl rounded-t-xl rounded-b-xl overflow-hidden place-items-center">
        <img :src="require('../assets/owner-min.png')">
        </div>
      <div class="home--catalog4 rounded-b lg:rounded-b-none lg:rounded-r flex flex-col place-items-center leading-normal">
          <div class="mb-7 ml-6">
            <div class="home--title text-gray-900 font-bold text-6xl text-left">Sungkono</div>
              <p class="home--title font-bold text-gray-400 text-left text-2xl mt-16">Owner</p>
              <p class="border-solid border border-blue-900"></p>
              <p class="text-gray-700 text-base text-left">Kami berkomitmen untuk memberikan yang terbaik kepada anda dengan memperhatikan keselamatan, kualitas dan kepuasan dengan terus memperbarui sistem kami untuk memastikan project berjalan lancar dan efisien.</p>
          </div>
        </div>
      </div>
    </div>
    
    <div class="imgPartners flex flex-col justify-center items-center w-full mb-14">
      <div class="home--title_isi mb-8 text-3xl">CLIENTS & PARTNERS</div>
      <!-- start swiper -->
      <div class="swiper swiper2 swiper-partners">
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
        // {
        //   url:"partners-9.png",
        //   tag:"partners",
        // },
        // {
        //   url:"partners-10.png",
        //   tag:"partners",
        // },
        // {
        //   url:"partners-11.png",
        //   tag:"partners",
        // },
        // {
        //   url:"partners-12.png",
        //   tag:"partners",
        // },
        // {
        //   url:"partners-13.png",
        //   tag:"partners",
        // },
        // {
        //   url:"partners-14.png",
        //   tag:"partners",
        // },
        // {
        //   url:"partners-15.png",
        //   tag:"partners",
        // },
        // {
        //   url:"partners-16.png",
        //   tag:"partners",
        // },
        // {
        //   url:"partners-17.png",
        //   tag:"partners",
        // },
        // {
        //   url:"partners-18.png",
        //   tag:"partners",
        // }
      ]
    }
  },
  

  methods:{
    initSwiperTest(){
      // eslint-disable-next-line
        this.swiperTest = new Swiper('.swiper-home', {
        // autoHeight: false,
        centeredSlides: true,
        slidesPerView: 3,
        spaceBetween: -80,
        loop: false,
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
          slidesPerView: 5.3,
          navigation: {
            nextEl: ".swiper-button-next-partners",
            prevEl: ".swiper-button-prev-partners"
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
  font-family: 'Montserrat, Inter';
  background: white;
  margin-top: -1px;

  &--title{
      font-family: 'Montserrat';
    }

  &--title_isi{
     font-family: 'Cabin';
     letter-spacing: 4px;
   }

  &--download{
      padding: 20px 64px;
      background-color: #0E1C4B;
      transition: 0.5s;
      color: white;
      font-family: 'Inter';
      font-weight: 700;
      font-size: 18px;
      border-radius: 4px;
      font-family: 'Cabin';
      letter-spacing: 4px;
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
      top: 60px;
      left: 1180px;
      background-image: url('../assets/ornament/insider7.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 152.02px;
      height: 158.76px;
      }
    }

    &--catalog2{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: 570px;
      left: -720px;
      background-image: url('../assets/ornament/insider3.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 154px;
      height: 360px;
      transform: rotate(180deg);
      }
    }

    &--catalog3{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: -40px;
      left: 620px;
      background-image: url('../assets/ornament/insider2.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 8px;
      height: 396px;
      transform: rotate(90deg);
      }
    }

    &--catalog4{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: 20px;
      left: 660px;
      background-image: url('../assets/ornament/insider.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 206px;
      height: 172px;
      transform: rotate(180deg);
      }
    }

}
.swiper{
  //background-color: #ffffff;
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
    img{
      object-fit: contain;
    }

    &.swiper-slide-active {
      background: white;
      opacity:1;
      transform: scale(1);
      z-index: 3;
    }

		
}

.swiper2{
    max-width: 1200px;
  }

.swiper-button-next,.swiper-button-prev{
    top: -100px;
  }
  .swiper-button-next{
    // position: relative;
    right: 50px;
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
    left: 50px;
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

    &.swiper-slide-active {
      background:white;
      opacity:1;
      // transform: scale(1);
      z-index: 3;
    }

		
}


img{
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;

  &--owner{
    height: 1035;
    width: 722;
  }
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






</style>
