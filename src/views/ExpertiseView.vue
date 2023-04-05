<template>
    <div class="expertise w-full relative px-4 xl:mx-auto"> 
        <!-- mulai dari sini -->
        <!-- MEKANIKAL & ELEKTRIKAL -->
        <div class="expertise--ornament1 w-full h-full"></div>
        <div class="flex flex-col justify-center items-center w-full mb-14">
          <div class="mb-8 text-3xl text-center font-bold">MEKANIKAL & ELEKTRIKAL</div>
          <div class="text-xl flex items-center text-center mb-8 max-w-5xl">
            <p>Kami menyediakan jasa dalam bidang Mekanikal dan Elektrikal. Pengalaman kami dalam mengelola kabel & jaringan seperti lampu runway pesawat,  SQFL (Sequence Flashing Light), Welder DPPU (Depot Pengisian Pesawat Udara), Apron Flood Light (penangkal petir & obstruction light) dan lainnya.</p>
          </div>
          <div class="mb-8">
             <!-- start swiper mekanikal -->
            <div class="swiper swiper-mekanikal">
              <div class="swiper-wrapper">
                <div class="swiper-slide" v-for="(index, key) in dataFotoMekanikal" :key="key">
                    <img :src="require(`../assets/mekanikElektrikal/${index.url}`)"/>
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
        <div class="expertise--ornament2 w-full h-full"></div>

        <!-- BIDANG TELEMATIKA -->
        <div class="flex flex-col justify-center items-center w-full mb-14 lg:mb-0 lg:mt-40 lg:pb-24">
          <div class="mb-8 text-3xl text-center font-bold">BIDANG TELEMATIKA</div>
          <div class="text-xl flex items-center text-center mb-8 max-w-5xl">Kami menyediakan jasa dalam bidang Telematika. Pengalaman kami dalam instalasi dan pemeliharaan CCTV & Penguat Signal Indoor Radio IGCS. PT. Bayur Jaya untuk melaksanakan instalasi jaringan kabel listrik, kabel optik, panel kontrol dan memasang serta melakukan pengaturan sebanyak 77+ titik kamera.</div>
          <div class="mb-8">
             <!-- start swiper telematika -->
            <div class="swiper swiper-telematika">
              <div class="swiper-wrapper">
                <div class="swiper-slide" v-for="(index, key) in dataFotoTelematika" :key="key">
                    <img :src="require(`../assets/bidangTelematika/${index.url}`)"/>
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
            url:"apron_ponti.jpg",
            category: "apron",
          },
          {
            url:"apron_ponti2.jpg",
            category: "apron",
          },
          {
            url:"apron_ponti3.jpg",
            category: "apron",
          },
          {
            url:"apron_ponti4.jpg",
            category: "apron",
          },
          {
            url:"apron_ponti5.jpg",
            category: "apron",
          },
          {
            url:"apron_ponti6.jpg",
            category: "apron",
          },
          {
            url:"bhs1.jpg",
            category: "bhs",
          },
          {
            url:"bhs2.jpg",
            category: "bhs",
          },
          {
            url:"bhs3.jpg",
            category: "bhs",
          },
          {
            url:"bhs4.jpg",
            category: "bhs",
          },
          {
            url:"bhs5.jpg",
            category: "bhs",
          },
          {
            url:"bhs6.jpg",
            category: "bhs",
          },
          {
            url:"bhs7.jpg",
            category: "bhs",
          },
          {
            url:"bhs8.jpg",
            category: "bhs",
          },
          {
            url:"bhs9.jpg",
            category: "bhs",
          },
          {
            url:"Kajar.jpg",
            category: "kajar",
          },
          {
            url:"Kajar1.jpg",
            category: "kajar",
          },
          {
            url:"Kajar2.jpg",
            category: "kajar",
          },
          {
            url:"Kajar3.jpg",
            category: "kajar",
          },
          {
            url:"Kajar4.jpg",
            category: "kajar",
          },
          {
            url:"Kajar5.jpg",
            category: "kajar",
          },
          {
            url:"Kajar6.jpg",
            category: "kajar",
          },
          {
            url:"Kajar7.jpg",
            category: "kajar",
          },
          {
            url:"Kajar8.jpg",
            category: "kajar",
          },
          {
            url:"pjuk1.jpg",
            category: "pjuk",
          },
          {
            url:"pjuk2.jpg",
            category: "pjuk",
          },
          {
            url:"pjuk3.jpg",
            category: "pjuk",
          },
          {
            url:"pjuk4.jpg",
            category: "pjuk",
          },
          {
            url:"pjuk5.jpg",
            category: "pjuk",
          },
          {
            url:"pjuk6.jpg",
            category: "pjuk",
          },
          {
            url:"ptm.jpg",
            category: "ptm",
          },
          {
            url:"ptm2.jpg",
            category: "ptm",
          },
          {
            url:"ptm3.jpg",
            category: "ptm",
          },
          {
            url:"ptm4.jpg",
            category: "ptm",
          },
          {
            url:"ptm5.jpg",
            category: "ptm",
          },
          {
            url:"ptm6.jpg",
            category: "ptm",
          },
          {
            url:"rtil1.jpg",
            category: "rtil",
          },
          {
            url:"rtil2.jpg",
            category: "rtil",
          },
          {
            url:"rtil3.jpg",
            category: "rtil",
          },
          {
            url:"rtil4.jpg",
            category: "rtil",
          },
          {
            url:"rtil5.jpg",
            category: "rtil",
          },
          {
            url:"rtil6.jpg",
            category: "rtil",
          },
          {
            url:"sqfl_thaha1.jpg",
            category: "sqfl",
          },
          {
            url:"sqfl_thaha2.jpg",
            category: "sqfl",
          },
          {
            url:"sqfl_thaha3.jpg",
            category: "sqfl",
          },
          {
            url:"sqfl_thaha4.jpg",
            category: "sqfl",
          },
          {
            url:"sqfl_thaha5.jpg",
            category: "sqfl",
          },
          {
            url:"sqfl_thaha6.jpg",
            category: "sqfl",
          },
          {
            url:"sqfl.jpg",
            category: "sqfl",
          },
          {
            url:"sqfl2.jpg",
            category: "sqfl",
          },
          {
            url:"sqfl3.jpg",
            category: "sqfl",
          },
          {
            url:"sqfl4.jpg",
            category: "sqfl",
          },
          {
            url:"sqfl5.jpg",
            category: "sqfl",
          },
          {
            url:"sqfl6.jpg",
            category: "sqfl",
          },
        ],
        dataFotoTelematika:[
          {
            url:"acu1.jpg",
            category: "acu",
          },
          {
            url:"acu2.jpg",
            category: "acu",
          },
          {
            url:"acu3.jpg",
            category: "acu",
          },
          {
            url:"acu4.jpg",
            category: "acu",
          },
          {
            url:"acu5.jpg",
            category: "acu",
          },
          {
            url:"acu6.jpg",
            category: "acu",
          },
          {
            url: "cct2.jpg",
            category: "cctv",
          },
          {
            url: "cct3.jpg",
            category: "cctv",
          },
          {
            url: "cct4.jpg",
            category: "cctv",
          },
          {
            url: "cct5.jpg",
            category: "cctv",
          },
          {
            url: "cct6.jpg",
            category: "cctv",
          },
          {
            url: "cct7.jpg",
            category: "cctv",
          },
          {
            url: "cctv-1.jpg",
            category: "cctv",
          },
          {
            url: "cctv-3.jpg",
            category: "cctv",
          },
          {
            url: "cctv-4.jpg",
            category: "cctv",
          },
          {
            url: "cctv-5.jpg",
            category: "cctv",
          },
          {
            url: "cctv-6.jpg",
            category: "cctv",
          },
          {
            url: "cctv-7.jpg",
            category: "cctv",
          },
          {
            url: "hytera.jpg",
            category: "hytera",
          },
          {
            url: "hytera2.jpg",
            category: "hytera",
          },
          {
            url: "hytera3.jpg",
            category: "hytera",
          },
          {
            url: "hytera5.jpg",
            category: "hytera",
          },
          {
            url: "hytera7.jpg",
            category: "hytera",
          },
          {
            url: "hytera8.jpg",
            category: "hytera",
          },
          {
            url: "Radar1.jpg",
            category: "radar",
          },
          {
            url: "Radar2.jpg",
            category: "radar",
          },
          {
            url: "Radar3.jpg",
            category: "radar",
          },
          {
            url: "Radar4.jpg",
            category: "radar",
          },
          {
            url: "Radar5.jpg",
            category: "radar",
          },
          {
            url: "Radar6.jpg",
            category: "radar",
          }
        ],
         
        
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
          //slidesPerView: 3,

          breakpoints: {
            480: {
              slidesPerView: 1.3,
              spaceBetween: 25
            },
            768: {
              slidesPerView: 3,
              spaceBetween: 30,
            },
            1280: {
              slidesPerView: 3,
              spaceBetween: 30,
            }
          },

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
          //slidesPerView: 3,
          breakpoints: {
            480: {
              slidesPerView: 1.3,
              spaceBetween: 25
            },
            768: {
              slidesPerView: 3,
              spaceBetween: 30,
            },
            1280: {
              slidesPerView: 3,
              spaceBetween: 30,
            }
          },
          
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

    &--ornament1{
      position: relative;
      &:before{
        content: "";
        position: absolute;
        bottom: -100px;
        right: 50px;
        background: #0a2753;
        border-radius: 50%;
        width: 80px;
        height: 80px;
        @include smartphone{
          display: none;
        }
      }
    }
    &--ornament2{
      position: relative;
      &:before{
        content: "";
        position: absolute;
        top: 0px;
        left: -20px;
        background-image: url('../assets/ornament/exp1.png');
        background-repeat: no-repeat;
        background-size: contain;
        width: 300px;
        height: 64px;
        @include smartphone{
          width: 150px;
          height: 32px;
          left: -16px;
          top: -45px;
        }
      }
    }

  }
  .swiper{
    max-width: 1000px;
    @include smartphone{
      max-width: 300px;
    }
  }

  .swiper-slide-active{
    &:hover{
      transform: scale(1.2);
    }
  }

  .swiper-button-next,.swiper-button-prev{
    top: -100px;
    box-shadow: 0px 2px 30px rgba(0,0,0,.4);
  }
  .swiper-button-next{
    // position: relative;
    right: -15px;
    @include smartphone{
      right: 3px;
    }
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
    left: -15px;
    @include smartphone{
      left: 3px;
    }
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