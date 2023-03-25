<template>
    <div class="contact w-full relative px-4 xl:px-48">
        <!-- mulai dari sini -->

      <div class="container mx-auto">
        <div class="grid grid-cols-1 gap md:grid-cols-2 lg:grid-cols-3">

        <!-- <div class="flex contact--title text-xl font-semibold w-48 h-7 left-44 top-60 text-center">KANTOR PUSAT</div>
        <div class="flex contact--title text-xl font-semibold w-48 h-7 left-44 top-60 text-center">WORKSHOP</div>
        <div class="flex contact--title text-xl font-semibold w-48 h-7 left-44 top-60 text-center">DIVISI TELKOM</div>
        <div class="flex contact--title_isi text-base text-justify w-60 mt-4"><img class="img--asset float-left mb-14 mr-4" :src="require('../assets/ornament/pin.png')">Jl. Raya Bayur No. 72 Periuk Jaya Tangerang Banten 15131</div>
        <div class="flex contact--title_isi text-base text-justify w-60 mt-4"><img class="img--asset float-left mb-14 mr-4" :src="require('../assets/ornament/pin.png')">Kp. Sekarwangi No. 39-40 Neglasari Tangerang Banten 15129</div>
        <div class="flex contact--title_isi text-base text-justify w-60 mt-4"><img class="img--asset float-left mb-14 mr-4" :src="require('../assets/ornament/pin.png')">Jl. Mandanau Blok A5 No 29 Tangerang Banten 15133</div>
        <div class="flex contact--title_isi text-base text-justify w-60 mt-3" v-for="(index, key) in dataEmail" :key="key">
                    <img :src="require(`../assets/ornament/mail.png`)" class="img--asset float-left mb-4 mr-4"/><a href="mailto:info@bayurjaya.co.id?subject=Mail from Our Site">info@bayurjaya.co.id</a>
          </div>
        <div class="flex contact--title_isi text-base text-justify w-60 mt-3"><img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')"><a href="tel:0215526610">+62 21 552 6610</a></div>
        <div class="flex contact--title_isi text-base text-justify w-60 mt-3"><img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')"><a href="tel:0215526610">+62 21 552 6610</a></div>
        <div class="flex contact--title_isi text-base text-justify w-60 mt-3"><img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')"><a href="tel:0215907462">+62 21 590 7462</a></div>
        <div class="flex contact--title_isi text-base text-justify w-60 mt-3" v-for="(index, key) in dataClock" :key="key">
                    <img :src="require(`../assets/ornament/clock.png`)" class="img--asset float-left mb-4 mr-4"/>Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00
          </div> -->

          <div>
          <div class="contact--title text-xl font-semibold w-48 h-7 left-44 top-60 mb-10 text-center underline underline-offset-8 decoration-4 decoration-blue-900">KANTOR PUSAT</div>
          <div class="contact--title_isi text-base text-justify w-60 mt-4 mb-10">
            <img class="img--asset float float-left mb-4 mr-4" :src="require('../assets/ornament/pin.png')">Jl. Raya Bayur No. 72 Periuk Jaya Tangerang Banten 15131</div>
          <div class="contact--title_isi text-base text-justify w-60 mb-8 mt-4">
            <img class="img--asset float float-left mb-4 mr-4" :src="require('../assets/ornament/mail.png')"><a href="mailto:info@bayurjaya.co.id?subject=Mail from Our Site">info@bayurjaya.co.id</a></div>
          <div class="contact--title_isi text-base text-justify w-60 mb-8 mt-4">
            <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')"><a href="tel:0215526610">+62 21 552 6610</a></div>
            <div class="contact--title_isi text-base text-justify w-60 mb-8 mt-4">
            <img class="img--asset float-left mb-10 mr-4 mt-3" :src="require('../assets/ornament/clock.png')">Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00</div>
        </div>
        <div>
          <div class="contact--title col-span-2 text-xl font-semibold w-48 h-7 left-44 top-60 mb-10 underline underline-offset-8 decoration-4 decoration-blue-900">WORKSHOP</div>
          <div class="contact--title_isi text-base text-justify w-60 mb-4 mt-4">
            <img class="img--asset float-left mb-10 mr-4" :src="require('../assets/ornament/pin.png')">Kp. Sekarwangi No. 39-40 Neglasari Tangerang Banten 15129</div>
          <div class="contact--title_isi text-base text-justify w-60 mt-4 mb-8">
            <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/mail.png')"><a href="mailto:info@bayurjaya.co.id?subject=Mail from Our Site">info@bayurjaya.co.id</a></div>
          <div class="contact--title_isi text-base text-justify w-60 mt-4 mb-8">
            <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')"><a href="tel:0215526610">+62 21 552 6610</a></div>
            <div class="contact--title_isi text-base text-justify w-60 mt-4 mb-8">
            <img class="img--asset float-left mb-10 mr-4 mt-3" :src="require('../assets/ornament/clock.png')">Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00</div>
        </div>
        <div>
          <div class="contact--title col-span-2 text-xl font-semibold w-48 h-7 left-44 top-60 mb-10 underline underline-offset-8 decoration-4 decoration-blue-900">DIVISI TELKOM</div>
          <div class="contact--title_isi text-base text-justify w-60 mt-4 mb-10">
            <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/pin.png')">Jl. Mandanau Blok A5 No 29 Tangerang Banten 15133</div>
          <div class="contact--title_isi text-base text-justify w-60 mt-4 mb-8">
            <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/mail.png')"><a href="mailto:info@bayurjaya.co.id?subject=Mail from Our Site">info@bayurjaya.co.id</a></div>
          <div class="contact--title_isi text-base text-justify w-60 mt-4 mb-8">
            <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')"><a href="tel:0215907462">+62 21 590 7462</a></div>
            <div class="contact--title_isi text-base text-justify w-60 mt-4 mb-8">
            <img class="img--asset float-left mb-10 mr-4 mt-3" :src="require('../assets/ornament/clock.png')">Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00</div>
        </div>
      


        </div>

        

     </div>
     <div class="grid grid-rows-2 gap-3">
     <div  class="row-span-1 contact--title text-3xl font-semibold not-italic mt-24">Deskripsikan Kebutuhan Anda, Kami Selalu Siap Membantu</div>
     <div  class="row-span-1 contact--title_isi font-semibold text-base not-italic mt-2 text-center">Kami menjamin bahwa semua data koresponden adalah bersifat RAHASIA dan tidak akan dipublikasikan.</div>
     </div>
     </div>
</template>

<script>
export default {
    name: 'ContactView',
    components: {
    },
    data(){
      return{
        email: null,
        clock: null,

        dataEmail:[{
            url:"email.png",
            category: "email",
        },
        {
            url:"email.png",
            category: "email",
        },
        {
            url:"email.png",
            category: "email",
        }
            
        ],

        dataClock:[{
            url:"clock.png",
            category: "clock",
        },
        {
            url:"clock.png",
            category: "clock",
        },
        {
            url:"clock.png",
            category: "clock",
        }
            
        ],


  
      }
    },
    methods:{
      initEmail(){
      // eslint-disable-next-line
        this.email = new email('.email-bayur', {
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
        });
      },

      initClock(){
      // eslint-disable-next-line
        this.clock = new clock('.clock-bayur', {
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
        });
      },
  
    },
    mounted(){
      this.initEmail()
      this.initClock()
    }
  }
</script>
<style lang="scss" scoped>

.contact{
  font-family: 'Montserrat, Inter';
  background: white;
  margin-top: -1px;

  &--title{
      font-family: 'Montserrat';
      font-weight: 600;
      text-align: center;
    }

  &--title_isi{
     font-family: 'Cabin';
     //text-align: center;
     //font-weight: 400;
   }
}

// .email{
//     max-width: 1000px;
//     @include smartphone{
//       max-width: 300px;
//     }
//   }

img{
  //width: 100%;
  //height: 100%;
  object-fit: contain;

  &--asset{
    position: relative;
    width: 24px;
    height: 24px;
    left: 186px;
    top: 327px;
    float: left;
    //bottom: 56px;
  }

}
  
</style>