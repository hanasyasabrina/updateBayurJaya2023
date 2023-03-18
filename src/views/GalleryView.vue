<template>
    <div class="gallery w-full relative px-48"> 
        <!-- mulai dari sini -->
        <!-- CCTV & KABEL JARINGAN -->
        <div class="flex flex-col justify-center items-center w-full mb-14">
          <div class="mb-8 text-3xl">CCTV & KABEL JARINGAN</div>
          <div class="mb-8">
             <!-- start swiper runway -->
            <div class="swiper swiper-cctv">
              <div class="swiper-wrapper">
                <div class="swiper-slide" v-for="(index, key) in dataFotoCCTV" :key="key">
                    <img :src="require(`../assets/gallery/cctvKabel/${index.url}`)"/>
                </div>
              </div>
             
            </div>
            <div class="w-full h-full relative">
              <div class="swiper-button-prev swiper-button-prev-cctv"></div>
              <div class="swiper-button-next swiper-button-next-cctv"></div>
            </div>

            <!-- end swiper -->
          </div>
          <div class="text-xl flex items-center text-center">Kami menyediakan jasa dalam bidang Telematika. Pengalaman kami dalam instalasi dan pemeliharaan CCTV & Penguat Signal Indoor Radio IGCS. PT. Bayur Jaya untuk melaksanakan instalasi jaringan kabel listrik, kabel optik, panel kontrol dan memasang serta melakukan pengaturan sebanyak 77+ titik kamera.</div>
        </div>

        <!-- RUNWAY & GARDU -->
        <div class="flex flex-col justify-center items-center w-full mb-14">
          <div class="mb-8 text-3xl">RUNWAY, GARDU & DPPU</div>
          <div class="mb-8">
             <!-- start swiper runway -->
            <div class="swiper swiper-runway">
              <div class="swiper-wrapper">
                <div class="swiper-slide" v-for="(index, key) in dataFotoRunway" :key="key">
                    <img :src="require(`../assets/gallery/runwayGardu/${index.url}`)"/>
                </div>
              </div>
            </div>
            <div class="w-full h-full relative">
              <div class="swiper-button-prev swiper-button-prev-runway "></div>
              <div class="swiper-button-next swiper-button-next-runway"></div>
            </div>
            <!-- end swiper -->
          </div>
          <div class="text-xl flex items-center text-center">Kami menyediakan jasa dalam bidang Telematika. Pengalaman kami dalam instalasi dan pemeliharaan CCTV & Penguat Signal Indoor Radio IGCS. PT. Bayur Jaya untuk melaksanakan instalasi jaringan kabel listrik, kabel optik, panel kontrol dan memasang serta melakukan pengaturan sebanyak 77+ titik kamera.</div>
        </div>

        <!-- SIPIL & TENAGA -->
        <div class="flex flex-col justify-center items-center w-full mb-14">
          <div class="mb-8 text-3xl">SIPIL</div>
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
          <div class="text-xl flex items-center text-center">Kami menyediakan jasa dalam bidang Telematika. Pengalaman kami dalam instalasi dan pemeliharaan CCTV & Penguat Signal Indoor Radio IGCS. PT. Bayur Jaya untuk melaksanakan instalasi jaringan kabel listrik, kabel optik, panel kontrol dan memasang serta melakukan pengaturan sebanyak 77+ titik kamera.</div>
        </div>
        <!-- BORING HDD -->
        <div class="flex flex-col justify-center items-center w-full mb-14">
          <div class="mb-8 text-3xl">HDD</div>
          <div class="mb-8">
             <!-- start swiper hdd -->
            <div class="swiper swiper-hdd">
              <div class="swiper-wrapper">
                <div class="swiper-slide" v-for="(index, key) in dataFotoHdd" :key="key">
                    <img :src="require(`../assets/gallery/boringHDD/${index.url}`)"/>
                </div>
              </div>
            </div>
            <div class="w-full h-full relative">
              <div class="swiper-button-prev swiper-button-prev-hdd"></div>
              <div class="swiper-button-next swiper-button-next-hdd"></div>
            </div>
            <!-- end swiper -->
          </div>
          <div class="text-xl flex items-center text-center">Kami menyediakan jasa dalam bidang Telematika. Pengalaman kami dalam instalasi dan pemeliharaan CCTV & Penguat Signal Indoor Radio IGCS. PT. Bayur Jaya untuk melaksanakan instalasi jaringan kabel listrik, kabel optik, panel kontrol dan memasang serta melakukan pengaturan sebanyak 77+ titik kamera.</div>
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
            url:"Radar2.jpeg",
            category: "runway",
          },
          {
            url:"Radar4.jpeg",
            category: "runway",
          },
          {
            url:"Radar6.jpeg",
            category: "runway",
          },
          {
            url:"rtil3.jpeg",
            category: "runway",
          },
          {
            url:"rtil6.jpeg",
            category: "runway",
          },
          {
            url:"sqfl2.jpeg",
            category: "runway",
          },
          {
            url:"Thaha.jpeg",
            category: "runway",
          },
          {
            url:"Thaha3.jpeg",
            category: "runway",
          }
        ],
        dataFotoCCTV:[
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
          dataFotoSipil:[
          {
            url:"sipil1.jpeg",
            category: "bb",
          },
          {
            url:"sipil2.jpeg",
            category: "bb1",
          },{
            url:"sipil3.jpeg",
            category: "cw5",
          },{
            url:"sipil4.jpeg",
            category: "gardu",
          },{
            url:"sipil5.jpeg",
            category: "sipil5",
          },{
            url:"Tank-1.jpeg",
            category: "Tank1",
          },{
            url:"Tank-4.jpeg",
            category: "Tank4",
          },{
            url:"Tank-7.jpeg",
            category: "Tank7",
          }],

          dataFotoHdd:[
          {
            url:"Hole2.jpeg",
            category: "hdd",
          },
          {
            url:"Hole3.jpeg",
            category: "hdd",
          },{
            url:"Hole4.jpeg",
            category: "hdd",
          },{
            url:"Hole7.jpeg",
            category: "hdd",
          }],

        
      }
    },
    methods:{
      initSwiperRunway(){
      // eslint-disable-next-line
        this.swiperRunway = new Swiper('.swiper-runway', {
          spaceBetween: 30,
          autoHeight: false,
          centeredSlides: true,
          loop: true,
          slidesPerView: 3,
          // If we need pagination
          pagination: {
            el: '.swiper-pagination',
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
          spaceBetween: 30,
          autoHeight: false,
          centeredSlides: true,
          loop: true,
          slidesPerView: 3,
          navigation: {
            nextEl: ".swiper-button-next-cctv",
            prevEl: ".swiper-button-prev-cctv"
          }
        });
      },
      initSwiperSipil(){
      // eslint-disable-next-line
        this.swiperSipil = new Swiper('.swiper-sipil', {
          spaceBetween: 30,
          autoHeight: false,
          centeredSlides: true,
          loop: true,
          slidesPerView: 3,
          navigation: {
            nextEl: ".swiper-button-next-sipil",
            prevEl: ".swiper-button-prev-sipil"
          }
        });
      },
      initSwiperHdd(){
      // eslint-disable-next-line
        this.swiperHDD = new Swiper('.swiper-hdd', {
          spaceBetween: 30,
          autoHeight: false,
          centeredSlides: true,
          loop: true,
          slidesPerView: 3,
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
  .gallery{
    margin-top: -1px;
    background-color: white;
  }
  .swiper{
    max-width: 1000px;
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
  </style>