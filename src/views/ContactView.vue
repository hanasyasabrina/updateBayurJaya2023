<template>
    <div class="contact w-full h-full relative xl:px-48">
        <!-- mulai dari sini -->

      <div class="container mx-auto">
        <div class="grid grid-cols-1 gap md:grid-cols-2 lg:grid-cols-3 pt-6">
          <div class="flex flex-col lg:justify-start justify-center lg:items-start items-center">
            <div class="contact--title text-xl font-semibold lg:ml-9 h-7 mb-6 text-center underline underline-offset-8 decoration-4 decoration-blue-900">KANTOR PUSAT</div>
            <div class="contact--title_isi text-base text-justify w-60 mb-6">
              <img class="img--asset float float-left mb-4 mr-4" :src="require('../assets/ornament/pin.png')">Jl. Raya Bayur No. 72 Periuk Jaya Tangerang Banten 15131</div>
            <div class="contact--title_isi text-base text-justify w-60 mb-4">
              <img class="img--asset float float-left mb-4 mr-4" :src="require('../assets/ornament/mail.png')"><a href="mailto:info@bayurjaya.com?subject=Mail from Our Site">info@bayurjaya.com</a></div>
            <div class="contact--title_isi text-base text-justify w-60 mb-4">
              <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')"><a href="tel:0215526610">+62 21 552 6610</a></div>
              <div class="contact--title_isi text-base text-justify w-60 mb-4">
              <img class="img--asset float-left mb-6 mr-4 mt-3" :src="require('../assets/ornament/clock.png')">Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00</div>
          </div>
          <div class="flex flex-col lg:justify-start justify-center lg:items-start items-center lg:mt-0 mt-16">
            <div class="contact--title col-span-2 text-xl font-semibold lg:ml-9 h-7 mb-6 underline underline-offset-8 decoration-4 decoration-blue-900">WORKSHOP</div>
            <div class="contact--title_isi text-base text-justify w-60 mb-4">
              <img class="img--asset float-left mb-8 mr-4" :src="require('../assets/ornament/pin.png')">Kp. Sekarwangi No. 39-40 Neglasari Tangerang Banten 15129</div>
            <div class="contact--title_isi text-base text-justify w-60 mb-4">
              <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/mail.png')"><a href="mailto:info@bayurjaya.com?subject=Mail from Our Site">info@bayurjaya.com</a></div>
            <div class="contact--title_isi text-base text-justify w-60 mb-4">
              <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')"><a href="tel:0215526610">+62 21 552 6610</a></div>
              <div class="contact--title_isi text-base text-justify w-60 mb-4">
              <img class="img--asset float-left mb-6 mr-4 mt-3" :src="require('../assets/ornament/clock.png')">Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00</div>
          </div>
          <div class="flex flex-col lg:justify-start justify-center lg:items-start items-center lg:mt-0 mt-16">
            <div class="contact--title col-span-2 text-xl font-semibold lg:ml-9 h-7 mb-6 underline underline-offset-8 decoration-4 decoration-blue-900">DIVISI TELKOM</div>
            <div class="contact--title_isi text-base text-justify w-60 mb-6">
              <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/pin.png')">Jl. Mandanau Blok A5 No 29 Tangerang Banten 15133</div>
            <div class="contact--title_isi text-base text-justify w-60 mb-4">
              <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/mail.png')"><a href="mailto:info@bayurjaya.com?subject=Mail from Our Site">info@bayurjaya.com</a></div>
            <div class="contact--title_isi text-base text-justify w-60 mb-4">
              <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')"><a href="tel:0215907462">+62 21 590 7462</a></div>
              <div class="contact--title_isi text-base text-justify w-60 mb-4">
              <img class="img--asset float-left mb-6 mr-4 mt-3" :src="require('../assets/ornament/clock.png')">Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00</div>
          </div>
        </div>
     </div>
      <div class="flex flex-col justify-center items-center mt-8 lg:px-0 px-4">
        <div class="contact--border"></div>
        <div  class="row-span-1 contact--title text-3xl font-semibold not-italic mt-16">Deskripsikan Kebutuhan Anda, Kami Selalu Siap Membantu</div>
        <div  class="row-span-1 contact--title_isi font-semibold text-base not-italic mt-2 text-center mb-16">Kami menjamin bahwa semua data koresponden adalah bersifat RAHASIA dan tidak akan dipublikasikan.</div>
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
   }
  &--border{
    width: 100%;
    max-width: 400px;
    border-top: 4px solid red;
    height: 4px;

  }
}


img{
  object-fit: contain;

  &--asset{
    position: relative;
    width: 24px;
    height: 24px;
    left: 186px;
    top: 327px;
    float: left;
  }

}
  
</style>