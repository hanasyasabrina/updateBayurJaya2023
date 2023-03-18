<template>
  <div class="home">
    <div class="font text-5xl w-full h-full flex justify-center font-extrabold">Build On Safety Is Our Foundation</div>
    <div class="font mx-80 flex text-center text-sm justify-center py-3">Kami adalah spesialis Jasa Konstruksi, Pengadaan Barang & Jasa dan Perdagangan Umum untuk pekerjaan dalam bidang Mekanikal & Elektrikal, Sipil, Telematika dan Jasa lainnya. Kami bangga dapat memberikan kualitas dan solusi luar biasa untuk klien terkemuka di seluruh Indonesia.</div>
    <!-- start swiper -->
    <div class="swiper">
      <div class="swiper-wrapper">
        <!-- Slides -->
        <div class="swiper-slide" v-for="(index, key) in dataFoto" :key="key">
            <img :src="require(`../assets/mekanikElektrikal/${index.url}`)"/>
        </div>
      </div>
      <!-- If we need pagination -->
      <div class="swiper-pagination"></div>
    </div>
    <!-- end swiper -->

    <div @click="testClick">
      <button class="font-inter bg-blue-900 hover:bg-gray-700 text-white py-2 px-4 rounded border-solid border-2 border-black">DOWNLOAD COMPANY PROFILE</button>
    </div>

    <div class="ml-96 pl-46 mr-96 my-8 border-solid border border-blue-900 place-items-right">

    </div>

    <div class="max-w-screen-md w-fit lg:max-w-screen-md lg:flex my-8 place-items-center mx-80">
    <div class="col-span-1 flex-none bg-cover object-contain rounded-xl rounded-t-xl rounded-b-xl h-72 w-48 overflow-hidden place-items-center">
      <img :src="require('../assets/owner-min.jpg')">
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
    <div class="bg-white mt-10 w-full h-full">CLIENTS & PARTNERS</div>
    <!-- start swiper -->
    <div class="swiper">
      <div class="swiper-wrapper">
        <!-- Slides -->
        <div class="swiper-slide-2" v-for="(index, key) in dataPartners" :key="key">
            <img :src="require(`../assets/partners/${index.url}`)"/>
        </div>
      </div>

      <!-- If we need pagination -->
      <div class="swiper-navigation"></div>
    </div>
    <!-- end swiper -->
    <!-- <div @click="testClick" v-for="(key, index) in dataFoto" :key="key">{{ index.url }}</div> -->
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
          url:"bidang1.png",
          tag: "mekanikal",
        },
        {
          url:"bidang2.png",
          tag: "cctv",
        },
        {
          url:"bidang3.png",
          tag: "sipil",
        }
      ],

      swiperPartners: null,
      dataPartners:[
        {
          url:"partners-1.png",
          tag:"honeywell",
        },
        {
          url:"partners-2.png",
          tag:"pertamina",
        },
        {
          url:"partners-3.png",
          tag:"philips",
        },
        {
          url:"partners-4.png",
          tag:"hitachi",
        },
        {
          url:"partners-5.png",
          tag:"wika",
        },
        {
          url:"partners-6.png",
          tag:"milestone",
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
        this.swiperPartners = new Swiper('.swiper', {
        loop: false,
        spaceBetween: -60,
        autoHeight: false,
        centeredSlides: true,
        slidesPerView: 3,
        autoplay:{
          delay: 2000
        },
        
        

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

imgPartners{
  width: max-w-2xl;
  height: max-h-fit;
}

.font{
  font-family: 'Montserrat';

}





</style>
