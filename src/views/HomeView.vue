<template>
  <div class="home relative w-full px-4 lg:px-0">
    <div class="home--catalog flex flex-col justify-center items-center w-full mb-12">
          <div class="home--title my-8 lg:mb-8 text-5xl text-center max-w-5xl not-italic font-bold">Build On Safety Is Our Foundation</div>
          <div class="home__desc home__desc--title text-center w-full flex max-w-screen-lg font-normal text-base text-center"><p>Kami adalah spesialis Jasa Konstruksi, Pengadaan Barang & Jasa dan Perdagangan Umum untuk pekerjaan dalam bidang Mekanikal & Elektrikal, Sipil, Telematika dan Jasa lainnya. Kami bangga dapat memberikan kualitas dan solusi luar biasa untuk klien terkemuka di seluruh Indonesia.</p></div>
    </div>
    <div class="home--ornament1 w-full h-full"></div>

    <!-- start swiper -->
    <div class="swiper swiper-home w-full lg:max-w-5xl">
      <div class="swiper-wrapper max-h-[600px]">
        <!-- Slides -->
        <div class="swiper-slide slide-card" v-for="(index, key) in dataFoto" :key="key">
            <img :src="require(`../assets/homeAssets/${index.url}`)"/>
        </div>
      </div>
      <!-- If we need pagination -->
      <div class="swiper-pagination"></div>
    </div>
    <!-- end swiper -->
    <div class="home--ornament2 w-full h-full"></div>
    <div class="flex justify-center items-center flex-col my-14">
      <a href="/files/compro-Bayur-2023.pdf" download>
        <div class="home--download">DOWNLOAD COMPANY PROFILE</div>
      </a>
    </div>
    <div class="home--catalog3 relative flex mb-14 w-full">
      <div class="flex lg:flex-row flex-col my-10 justify-center lg:max-w-5xl max-w-[250px] mx-auto">
        <div class="img--owner mx-auto bg-cover object-contain rounded-xl rounded-t-xl rounded-b-xl overflow-hidden">
          <img class="w-full" :src="require('../assets/owner-min.png')">
        </div>
        <div class="home--catalog4 lg:justify-center lg:max-w-5xl rounded-b lg:rounded-r flex flex-col leading-normal">
          <div class="flex flex-col lg:mb-7 lg:ml-14">
            <div class="home--title text-gray-900 font-bold lg:text-6xl text-2xl text-left mt-6">Sungkono</div>
              <div class="home--title font-bold text-gray-400 text-left lg:text-2xl text-xl mt-6">Founder</div>
              <div class="border-solid border border-blue-900 lg:max-w-xs max-w-[100px] mb-4"></div>
              <div class="home__desc--owner text-base text-left max-w-xl">Kami berkomitmen untuk memberikan yang terbaik kepada anda dengan memperhatikan keselamatan, kualitas dan kepuasan dengan terus memperbarui sistem kami untuk memastikan project berjalan lancar dan efisien.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="home--ornament3 w-full h-full"></div>
    
    <div class="imgPartners flex flex-col justify-center items-center w-full mt-8 pb-14">
      <div class="home__desc home__desc--title mb-0 xl:text-3xl text-xl text-center">CLIENTS & PARTNERS</div>
      <!-- start swiper -->
      <div class="swiper swiper2 swiper-partners">
        <div class="swiper-wrapper items-center">
          <div class="swiper-slide slide-partners flex items-center justify-center" v-for="(index, key) in dataPartners" :key="key">
            <img class="img--partner" :src="require(`../assets/partners/${index.url}`)"/>
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

// import { disconnect } from 'process';

// import { container } from 'webpack';

export default {
  name: 'HomeView',
  components: {
    // disconnect
},
  data(){
    return{
      swiperTest: null,
      urlFile: 'http://localhost:8080/src/assets/files/compro-Bayur-2023.pdf',
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
        },
        {
          url:"partners-19.png",
          tag:"partners",
        },
        {
          url:"partners-20.png",
          tag:"partners",
        },
        {
          url:"partners-21.png",
          tag:"partners",
        },
        {
          url:"partners-22.png",
          tag:"partners",
        },
        {
          url:"partners-23.png",
          tag:"partners",
        },
        {
          url:"partners-24.png",
          tag:"partners",
        },
        {
          url:"partners-25.png",
          tag:"partners",
        },
        {
          url:"partners-26.png",
          tag:"partners",
        },
        {
          url:"partners-27.png",
          tag:"partners",
        },
        {
          url:"partners-28.png",
          tag:"partners",
        },
      ]
    }
  },
  

  methods:{
    initSwiperTest(){
      // eslint-disable-next-line
        this.swiperTest = new Swiper('.swiper-home', {
        // autoHeight: false,
        centeredSlides: true,
        // slidesPerView: 3,
        // spaceBetween: -80,
        loop: false,
        breakpoints: {
            480: {
              slidesPerView: 1.2,
              spaceBetween: -10
            },
            768: {
              slidesPerView: 3,
              spaceBetween: -30,
            },
            1280: {
              slidesPerView: 3,
              spaceBetween: -30,
            }
          },
        autoplay:{
          delay: 2000
        },
        // If we need pagination
        pagination: {
          el: '.swiper-pagination',
        },

      });
    },
    downloadFileLocal(response){
      const url = window.URL.createObjectURL(new Blob([response.data]))
      const link = document.createElement('a')
      link.href = url
      link.setAttribute('download', 'Compro Bayur Jaya 2023.pdf') //or any other extension
      document.body.appendChild(link)
      link.click()
    },
    downloadWithVueResource() {
      // eslint-disable-next-line
      axios({
        method: 'get',
        url: this.urlFile,
        responseType: 'blob'
      })
      .then(response => {
        this.downloadFileLocal(response)  
      })
      .catch(() => console.log('error occured'))
      
    },
    testClick(){
      alert('INI HASIL @ KLIK METHOD')
    },

    initSwiperPartners(){
      // eslint-disable-next-line
        this.swiperPartners = new Swiper('.swiper-partners', {
          // spaceBetween: 30,
          autoHeight: false,
          centeredSlides: true,
          loop: true,
          // slidesPerView: 5.3,
          breakpoints: {
            480: {
              slidesPerView: 1.3,
              spaceBetween: 50  
            },
            768: {
              slidesPerView: 3,
              spaceBetween: 30,
            },
            1280: {
              slidesPerView: 5.3,
              spaceBetween: 30,
            }
          },
          navigation: {
            nextEl: ".swiper-button-next-partners",
            prevEl: ".swiper-button-prev-partners"
          }
        });
      },
  },
  mounted(){
    this.initSwiperTest()
    this.initSwiperPartners()
  }
}
</script>

<!-- vue, tailwind, sass, swiper -->

<style lang="scss" scoped>
@mixin smartphone {
    @media (max-width: 599px) { @content; }
  }
.home{
  font-family: 'Montserrat, Inter';
  background: white;
  margin-top: -1px;

  &--title{
      font-family: 'Montserrat';
    }
  &__desc{
    font-family: 'Cabin';
    &--title{
      letter-spacing: 2px;
    }
    &--owner{
      letter-spacing: 1px;
    }
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
      cursor: pointer;
      @include smartphone{
        padding: 20px 48px;
        text-align: center;
      }
      &:hover{
        background-color: #4B0E0E;
      }
    }

  &--ornament1{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: -90px;
      right: 30px;
      background-image: url('../assets/ornament/home2.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 150px;
      height: 150px;
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
      left: 0px;
      background-image: url('../assets/ornament/home3.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 208px;
      height: 400px;
      @include smartphone{
        display: none;
      }
    }
  }
  &--ornament3{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: -150px;
      right: 65px;
      background-image: url('../assets/ornament/home1.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 150px;
      height: 150px;
      @include smartphone{
        display: none;
      }
    }
  }

}
.swiper{
  width: 100%;
  height: 100%;
  
}
.slide-card {
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
    max-width: 1000px;
    max-height: 250px;
  }

.swiper-button-next,.swiper-button-prev{
    top: -100px;
    box-shadow: 0px 2px 30px rgba(0,0,0,.4);
  }
  .swiper-button-next{
    right: 12%;
    @include smartphone{
      right: 5px;
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
    left: 12%;
    @include smartphone{
      left: 5px;
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

.slide-partners {
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
      width: 100%;
      height: 100%;
      object-fit: contain;
    }

    &.swiper-slide-active {
      background:white;
      opacity:1;
      z-index: 3;
      @include smartphone{
        transform: scale(.8);
      }
    }

		
}


img{
  display: block;
  width: 100%;
  height: 100%;
  object-fit: contain;

  

  &--owner{
    height: 1035;
    width: 722;
  }
}
.img--partner{
    max-height: 250px;
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
