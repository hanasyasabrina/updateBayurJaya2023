<template>
    <div class="expertise w-full relative px-4 xl:px-48"> 
        <!-- mulai dari sini -->
        <!-- MEKANIKAL & ELEKTRIKAL -->
        <div class="expertise--catalog flex flex-col justify-center items-center w-full mb-14">
          <div class="mb-8 text-3xl text-center">MEKANIKAL & ELEKTRIKAL</div>
          <div class="text-xl flex items-center text-justify mb-8 max-w-5xl">
            <p>Kami menyediakan jasa dalam bidang Mekanikal dan Elektrikal. Pengalaman kami dalam mengelola kabel & jaringan seperti lampu runway pesawat,  SQFL (Sequence Flashing Light), Welder DPPU (Depot Pengisian Pesawat Udara), Apron Flood Light (penangkal petir & obstruction light) dan lainnya.</p>
          </div>
          <div class="mb-8">
             <!-- start swiper mekanikal -->
            <div class="swiper swiper-mekanikal">
              <div class="swiper-wrapper">
                <div class="swiper-slide" v-for="(index, key) in dataFotoMekanikal" :key="key">
                    <img :src="require(`../assets/gallery/cctvKabel/${index.url}`)"/>
                </div>
              </div>
             
            </div>
            <div class="w-full h-full relative">
              <div class="swiper-button-prev swiper-button-prev-mekanikal"></div>
              <div class="swiper-button-next swiper-button-next-mekanikal"></div>
            </div>

            <!-- end swiper -->
          </div>
          
        </div>

        <!-- BIDANG TELEMATIKA -->
        <div class="flex flex-col justify-center items-center w-full mb-14">
          <div class="mb-8 text-3xl">BIDANG TELEMATIKA</div>
          <div class="text-xl flex items-center text-justify mb-8 max-w-5xl">Kami menyediakan jasa dalam bidang Telematika. Pengalaman kami dalam instalasi dan pemeliharaan CCTV & Penguat Signal Indoor Radio IGCS. PT. Bayur Jaya untuk melaksanakan instalasi jaringan kabel listrik, kabel optik, panel kontrol dan memasang serta melakukan pengaturan sebanyak 77+ titik kamera.</div>
          <div class="mb-8">
             <!-- start swiper telematika -->
            <div class="swiper swiper-telematika">
              <div class="swiper-wrapper">
                <div class="swiper-slide" v-for="(index, key) in dataFotoTelematika" :key="key">
                    <img :src="require(`../assets/gallery/cctvKabel/${index.url}`)"/>
                </div>
              </div>
            </div>
            <div class="w-full h-full relative">
              <div class="swiper-button-prev swiper-button-prev-telematika"></div>
              <div class="swiper-button-next swiper-button-next-telematika"></div>
            </div>
            <!-- end swiper -->
          </div>
          </div>
    </div>
  </template>
  <script>
  export default {
    name: 'ExpertiseView',
    components: {
      // HelloWorld
    },
    data(){
      return{
        swiperMekanikal: null,
        swiperTelematika: null,

        dataFotoMekanikal:[
        {
            url:"cct1.jpeg",
            category: "cctv",
          },
          {
            url:"cct3.jpeg",
            category: "cctv",
          },{
            url:"cct4.jpeg",
            category: "cctv",
          },{
            url:"cct5.jpeg",
            category: "cctv",
          },{
            url:"cctv-5.jpeg",
            category: "cctv",
          },{
            url:"cctv-7.jpeg",
            category: "cctv",
          }
        ],
        dataFotoTelematika:[
          {
            url:"cct1.jpeg",
            category: "cctv",
          },
          {
            url:"cct3.jpeg",
            category: "cctv",
          },{
            url:"cct4.jpeg",
            category: "cctv",
          },{
            url:"cct5.jpeg",
            category: "cctv",
          },{
            url:"cctv-5.jpeg",
            category: "cctv",
          },{
            url:"cctv-7.jpeg",
            category: "cctv",
          }],
         
        
        }
      
    },
    methods:{
      initSwiperMekanikal(){
      // eslint-disable-next-line
        this.swiperMekanikal = new Swiper('.swiper-mekanikal', {
          spaceBetween: 30,
          autoHeight: false,
          centeredSlides: true,
          loop: true,
          slidesPerView: 3,
          navigation: {
            nextEl: ".swiper-button-next-mekanikal",
            prevEl: ".swiper-button-prev-mekanikal"
          }
        });
      },
      initSwiperTelematika(){
      // eslint-disable-next-line
        this.swiperTelematika = new Swiper('.swiper-telematika', {
          spaceBetween: 30,
          autoHeight: false,
          centeredSlides: true,
          loop: true,
          slidesPerView: 3,
          navigation: {
            nextEl: ".swiper-button-next-telematika",
            prevEl: ".swiper-button-prev-telematika"
          }
        });
      }
      
    },
    mounted(){
      this.initSwiperMekanikal()
      this.initSwiperTelematika()
    }
  }
  </script>
  <style lang="scss" scoped>

@mixin smartphone {
    @media (max-width: 599px) { @content; }
  }
  .expertise{
    margin-top: -1px;
    background-color: white;

    &--catalog{
      position: relative;
      // &:before{
      //   content: "";
      //   position: absolute;
      //   top: -40px;
      //   left: 925px;
      //   background-image: url('../assets/ornament/insider4.png');
      //   background-repeat: no-repeat;
      //   background-size: contain;
      //   width: 54px;
      //   height: 54px;
      // }
    }
  }
  .swiper{
    max-width: 1000px;
    @include smartphone{
      max-width: 300px;
    }
  }

  .swiper-slide{
    &:hover{
      transform: scale(1.4);
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
      
      @include smartphone{
        padding: 75%;
      }
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

      @include smartphone{
        padding: 75%;
      }
    }
  }
  </style>