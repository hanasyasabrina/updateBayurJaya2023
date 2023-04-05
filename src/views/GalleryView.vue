<template>
    <div class="gallery w-full relative px-4 lg:px-0 xl:mx-auto"> 
        <!-- mulai dari sini -->
        <!-- CCTV & KABEL JARINGAN -->
        <div class="flex flex-col justify-center items-center w-full mb-14 py-12">
          <div class="mb-8 text-3xl text-center font-bold">CCTV & KABEL JARINGAN</div>
          <div class="mb-8">
             <!-- start swiper runway -->
            <div class="swiper swiper-cctv">
              <div class="swiper-wrapper">
                <div class="swiper-slide" v-for="(index, key) in dataFotoCCTV" :key="key">
                    <img :src="require(`../assets/bidangTelematika/${index.url}`)"/>
                </div>
              </div>
             
            </div>
            <div class="w-full h-full relative">
              <div class="swiper-button-prev swiper-button-prev-cctv"></div>
              <div class="swiper-button-next swiper-button-next-cctv"></div>
            </div>

            <!-- end swiper -->
          </div>
          <div class="text-xl flex items-center text-center max-w-5xl">
            <p>Kami menyediakan jasa dalam bidang Telematika. Pengalaman kami dalam instalasi dan pemeliharaan CCTV & Penguat Signal Indoor Radio IGCS. PT. Bayur Jaya untuk melaksanakan instalasi jaringan kabel listrik, kabel optik, panel kontrol dan memasang serta melakukan pengaturan sebanyak 77+ titik kamera.</p>
          </div>
        </div>
        <div class="gallery--ornament1 w-full h-full"></div>

        <!-- RUNWAY & GARDU -->
        <div class="flex flex-col justify-center items-center w-full mb-14 py-12">
          <div class="mb-8 text-3xl text-center font-bold">RUNWAY, GARDU & DPPU</div>
          <div class="mb-8">
             <!-- start swiper runway -->
            <div class="swiper swiper-runway">
              <div class="swiper-wrapper">
                <div class="swiper-slide" v-for="(index, key) in dataFotoRunway" :key="key">
                    <img :src="require(`../assets/mekanikElektrikal/${index.url}`)"/>
                </div>
              </div>
            </div>
            <div class="w-full h-full relative">
              <div class="swiper-button-prev swiper-button-prev-runway "></div>
              <div class="swiper-button-next swiper-button-next-runway"></div>
            </div>
            <!-- end swiper -->
          </div>
          <div class="text-xl flex items-center text-center max-w-5xl">Pekerjaan Penggantian Peralatan Sequence Flashing Light (SQFL) di Bandara Internasional Minangkabau dari konfigurasi 30 unit baru di ujung runway 33. Pekerjaan lainnya Apron Flood Light yang dilengkapi dengan penangkal petir dan obstruction light, sehingga dapat terlihat dari service road untuk memudahkan maintenance dikemudian hari.</div>
        </div>
        <div class="gallery--ornament2 w-full h-full"></div>

        <!-- SIPIL & TENAGA -->
        <div class="flex flex-col justify-center items-center w-full mb-14 py-12">
          <div class="mb-8 text-3xl font-bold">SIPIL & TENAGA</div>
          <div class="mb-8">
             <!-- start swiper sipil -->
            <div class="swiper swiper-sipil">
              <div class="swiper-wrapper">
                <div class="swiper-slide" v-for="(index, key) in dataFotoSipil" :key="key">
                    <img :src="require(`../assets/gallery/sipilTenaga/${index.url}`)"/>
                </div>
              </div>
            </div>
            <div class="w-full h-full relative">
              <div class="swiper-button-prev swiper-button-prev-sipil"></div>
              <div class="swiper-button-next swiper-button-next-sipil"></div>
            </div>
            <!-- end swiper -->
          </div>
          <div class="text-xl flex items-center text-center max-w-5xl">
            <p>Salah satu kerja Sipil yang dikerjakan Bayur Jaya adalah Pembangunan Rumah Hunian Cluster LaVerde Serpong Park di Kota Tangerang Selatan dan Intstalasi Gardu T.03, T.08 dan T.10 Terminal 3 Bandara Internasional Soekarno-Hatta.</p>
          </div>
        </div>
        <div class="gallery--ornament3 w-full h-full"></div>
        <!-- BORING HDD -->
        <div class="flex flex-col justify-center items-center w-full mb-14 lg:mb-0 py-12">
          <div class="mb-8 text-3xl font-bold">BORING HDD</div>
          <div class="mb-8">
             <!-- start swiper hdd -->
            <div class="swiper swiper-hdd">
              <div class="swiper-wrapper">
                <div class="swiper-slide" v-for="(index, key) in dataFotoHdd" :key="key">
                    <img :src="require(`../assets/gallery/sipilTenaga/${index.url}`)"/>
                </div>
              </div>
            </div>
            <div class="w-full h-full relative">
              <div class="swiper-button-prev swiper-button-prev-hdd"></div>
              <div class="swiper-button-next swiper-button-next-hdd"></div>
            </div>
            <!-- end swiper -->
          </div>
          <div class="text-xl flex items-center text-center mb-8 max-w-5xl">Kami menyediakan jasa pelayanan sewa mesin bor HDD yang dapat digunakan untuk pemasangan jaringan kabel optik / listrik, pipa HDPE atau PE dan lainnya. Dengan menggunakan mesin bor HDD ini tidak perlu dilakukan penggalian jalan atau bangunan yang akan dilewati jalur instalasi kabel/pipa, sehingga dapat menghemat waktu dan biaya karena tidak memerlukan banyak tenaga manusia untuk melakukan penggalian sebagaimana pemasangan instalasi jaringan kabel/pipa secara manual.</div>
        </div>
       
    </div>
  </template>
  <script>
  export default {
    name: 'GalleryView',
    components: {
      // HelloWorld
    },
    data(){
      return{
        swiperRunway: null,
        swiperCCTV: null,
        swiperSipil: null,
        swiperHDD: null,

        dataFotoRunway:[
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
          }
        ],
        dataFotoCCTV:[
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
          }
        ],
          dataFotoSipil:[
          {
            url:"bb.jpg",
            category: "BB",
          },
          {
            url:"BB1.jpg",
            category: "BB",
          },
          {
            url:"BB2.jpg",
            category: "BB",
          },
          {
            url:"BB3.jpg",
            category: "BB",
          },
          {
            url:"BB4.jpg",
            category: "BB",
          },
          {
            url:"BB5.jpg",
            category: "BB",
          },
          {
            url:"BB6.jpg",
            category: "BB",
          },
          {
            url:"BB8.jpg",
            category: "BB",
          },
          {
            url:"BB9.jpg",
            category: "BB",
          },
          {
            url:"Hole1.jpg",
            category: "hdd",
          },
          {
            url:"Hole2.jpg",
            category: "hdd",
          },
          {
            url:"Hole3.jpg",
            category: "hdd",
          },
          {
            url:"Hole4.jpg",
            category: "hdd",
          },
          {
            url:"Hole5.jpg",
            category: "hdd",
          },
          {
            url:"Hole6.jpg",
            category: "hdd",
          },
          {
            url:"Hole7.jpg",
            category: "hdd",
          },
          {
            url:"laverde1.jpg",
            category: "laverde",
          },
          {
            url:"laverde2.jpg",
            category: "laverde",
          },
          {
            url:"laverde3.jpg",
            category: "laverde",
          },
          {
            url:"laverde4.jpg",
            category: "laverde",
          },
          {
            url:"laverde5.jpg",
            category: "laverde",
          },
          {
            url:"laverde6.jpg",
            category: "laverde",
          },
          {
            url:"meg1.jpg",
            category: "meg",
          },
          {
            url:"meg2.jpg",
            category: "meg",
          },
          {
            url:"meg3.jpg",
            category: "meg",
          },
          {
            url:"meg4.jpg",
            category: "meg",
          },
          {
            url:"meg5.jpg",
            category: "meg",
          },
          {
            url:"meg6.jpg",
            category: "meg",
          },
          {
            url:"Tank-1.jpg",
            category: "Tank",
          },{
            url:"Tank-2.jpg",
            category: "Tank",
          },{
            url:"Tank-3.jpg",
            category: "Tank",
          },
          {
            url:"Tank-4.jpg",
            category: "Tank",
          },
          {
            url:"Tank-5.jpg",
            category: "Tank",
          },
          {
            url:"Tank-7.jpg",
            category: "Tank",
          }
        ],

          dataFotoHdd:[
          {
            url:"Hole1.jpg",
            category: "hdd",
          },
          {
            url:"Hole2.jpg",
            category: "hdd",
          },
          {
            url:"Hole3.jpg",
            category: "hdd",
          },
          {
            url:"Hole4.jpg",
            category: "hdd",
          },
          {
            url:"Hole5.jpg",
            category: "hdd",
          },
          {
            url:"Hole6.jpg",
            category: "hdd",
          },
          {
            url:"Hole7.jpg",
            category: "hdd",
          }
        ],

        
      }
    },
    methods:{
      initSwiperRunway(){
      // eslint-disable-next-line
        this.swiperRunway = new Swiper('.swiper-runway', {
          autoHeight: false,
          centeredSlides: true,
          loop: true,
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
            nextEl: ".swiper-button-next-runway",
            prevEl: ".swiper-button-prev-runway"
          }
        });
      },
      initSwiperCCTV(){
      // eslint-disable-next-line
        this.swiperCCTV = new Swiper('.swiper-cctv', {
          // spaceBetween: 30,
          autoHeight: false,
          centeredSlides: true,
          loop: true,
          // slidesPerView: 3,
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
            nextEl: ".swiper-button-next-cctv",
            prevEl: ".swiper-button-prev-cctv"
          }
        });
      },
      initSwiperSipil(){
      // eslint-disable-next-line
        this.swiperSipil = new Swiper('.swiper-sipil', {
          autoHeight: false,
          centeredSlides: true,
          loop: true,
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
            nextEl: ".swiper-button-next-sipil",
            prevEl: ".swiper-button-prev-sipil"
          }
        });
      },
      initSwiperHdd(){
      // eslint-disable-next-line
        this.swiperHDD = new Swiper('.swiper-hdd', {
          autoHeight: false,
          centeredSlides: true,
          loop: true,
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
            nextEl: ".swiper-button-next-hdd",
            prevEl: ".swiper-button-prev-hdd"
          }
        });
      },
    },
    mounted(){
      this.initSwiperRunway()
      this.initSwiperCCTV()
      this.initSwiperSipil()
      this.initSwiperHdd()
    }
  }
  </script>
  <style lang="scss" scoped>
   @mixin smartphone {
    @media (max-width: 599px) { @content; }
  }
  .gallery{
    margin-top: -1px;
    background-color: white;

    &--ornament1{
      position: relative;
      &:before{
        content: "";
        position: absolute;
        top: 0px;
        right: 0px;
        background-image: url('../assets/ornament/gallery2.png');
        background-repeat: no-repeat;
        background-size: contain;
        width: 300px;
        height: 64px;
        @include smartphone{
          width: 150px;
          height: 32px;
          right: -16px;
          top: -45px;
        }
      }
    }

    &--ornament2{
      position: relative;
      &:before{
        content: "";
        position: absolute;
        top: 0px;
        left: 0px;
        background-image: url('../assets/ornament/gallery1.png');
        background-repeat: no-repeat;
        background-size: contain;
        width: 200px;
        height: 64px;
        @include smartphone{
          width: 100px;
          height: 32px;
          left: -16px;
          top: -45px;
        }
      }
    }

    &--ornament3{
      position: relative;
      &::before{
        content: "";
        position: absolute;
        top: 0;
        right: 85px;
        background-color: #e33c3a;
        border-radius: 8px;
        width: 450px;
        height: 8px;
        @include smartphone{
          top: -25px;
          width: 200px;
          height: 4px;
          right: -16px;
          border-top-left-radius: 8px;
          border-bottom-left-radius: 8px;
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
    right: -15px;
    @include smartphone{
      right: 3px;
    }
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