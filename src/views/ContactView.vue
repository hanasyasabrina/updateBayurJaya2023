<template>
    <div class="contact w-full relative px-4 xl:px-48">
        <!-- mulai dari sini -->

      <div class="grid grid-cols-3 gap">

        <div class="contact--title text-xl font-semibold w-48 h-7 left-44 top-60 text-center">KANTOR PUSAT</div>
        <div class="contact--title text-xl font-semibold w-48 h-7 left-44 top-60 text-center">WORKSHOP</div>
        <div class="contact--title text-xl font-semibold w-48 h-7 left-44 top-60 text-center">DIVISI TELKOM</div>
        <div class="contact--title_isi text-base text-justify w-60 mt-4"><img class="img--asset float-left mb-14 mr-4" :src="require('../assets/ornament/pin.png')">Jl. Raya Bayur No. 72 Periuk Jaya Tangerang Banten 15131</div>
        <div class="contact--title_isi text-base text-justify w-60 mt-4"><img class="img--asset float-left mb-14 mr-4" :src="require('../assets/ornament/pin.png')">Kp. Sekarwangi No. 39-40 Neglasari Tangerang Banten 15129</div>
        <div class="contact--title_isi text-base text-justify w-60 mt-4"><img class="img--asset float-left mb-14 mr-4" :src="require('../assets/ornament/pin.png')">Jl. Mandanau Blok A5 No 29 Tangerang Banten 15133</div>
        <div class="contact--title_isi text-base text-justify w-60 mt-3"><img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/mail.png')"><a href="mailto:info@bayurjaya.co.id?subject=Mail from Our Site">info@bayurjaya.co.id</a></div>
        <div class="contact--title_isi text-base text-justify w-60 mt-3"><img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/mail.png')"><a href="mailto:info@bayurjaya.co.id?subject=Mail from Our Site">info@bayurjaya.co.id</a></div>
        <div class="contact--title_isi text-base text-justify w-60 mt-3"><img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/mail.png')"><a href="mailto:info@bayurjaya.co.id?subject=Mail from Our Site">info@bayurjaya.co.id</a></div>
        <div class="contact--title_isi text-base text-justify w-60 mt-3"><img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')"><a href="tel:0215526610">+62 21 552 6610</a></div>
        <div class="contact--title_isi text-base text-justify w-60 mt-3"><img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')"><a href="tel:0215526610">+62 21 552 6610</a></div>
        <div class="contact--title_isi text-base text-justify w-60 mt-3"><img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')"><a href="tel:0215907462">+62 21 590 7462</a></div>
        <div class="contact--title_isi text-base text-justify w-60 mt-3"><img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/clock.png')">Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00</div>
        <div class="contact--title_isi text-base text-justify w-60 mt-3"><img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/clock.png')">Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00</div>
        <div class="contact--title_isi text-base text-justify w-60 mt-3"><img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/clock.png')">Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00</div>
        

        <!-- <div>
          <p class="contact--title text-xl font-semibold w-48 h-7 left-44 top-60 text-center">KANTOR PUSAT</p>
          <p class="contact--title_isi text-base text-justify w-60 mt-4">
            <img class="img--asset float-left mb-10 mr-4" :src="require('../assets/ornament/pin.png')">Jl. Raya Bayur No. 72 Periuk Jaya Tangerang Banten 15131</p>
          <p class="contact--title_isi text-base text-justify w-60 mt-4">
            <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/mail.png')">info@bayurjaya.co.id</p>
          <p class="contact--title_isi text-base text-justify w-60 mt-4">
            <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')">+62 21 552 6610</p>
            <p class="contact--title_isi text-base text-justify w-60 mt-4">
            <img class="img--asset float-left mb-4 mr-4 mt-3" :src="require('../assets/ornament/clock.png')">Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00</p>
        </div>
        <div>
          <p class="contact--title col-span-2 text-xl font-semibold w-48 h-7 left-44 top-60">WORKSHOP</p>
          <p class="contact--title_isi text-base text-justify w-60 mt-4">
            <img class="img--asset float-left mb-10 mr-4" :src="require('../assets/ornament/pin.png')">Kp. Sekarwangi No. 39-40 Neglasari Tangerang Banten 15129</p>
          <p class="contact--title_isi text-base text-justify w-60 mt-4">
            <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/mail.png')">info@bayurjaya.co.id</p>
          <p class="contact--title_isi text-base text-justify w-60 mt-4">
            <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')">+62 21 552 6610</p>
            <p class="contact--title_isi text-base text-justify w-60 mt-4">
            <img class="img--asset float-left mb-4 mr-4 mt-3" :src="require('../assets/ornament/clock.png')">Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00</p>
        </div>
        <div>
          <p class="contact--title col-span-2 text-xl font-semibold w-48 h-7 left-44 top-60">DIVISI TELKOM</p>
          <p class="contact--title_isi text-base text-justify w-60 mt-4">
            <img class="img--asset float-left mb-10 mr-4" :src="require('../assets/ornament/pin.png')">Jl. Mandanau Blok A5 No 29 Tangerang Banten 15133</p>
          <p class="contact--title_isi text-base text-justify w-60 mt-4">
            <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/mail.png')">info@bayurjaya.co.id</p>
          <p class="contact--title_isi text-base text-justify w-60 mt-4">
            <img class="img--asset float-left mb-4 mr-4" :src="require('../assets/ornament/telephone.png')">+62 21 590 7462</p>
            <p class="contact--title_isi text-base text-justify w-60 mt-4">
            <img class="img--asset float-left mb-4 mr-4 mt-3" :src="require('../assets/ornament/clock.png')">Senin – Jum’at. 8.00 – 17.00 Sabtu. 8.00 – 12.00</p>
        </div>
       -->

     </div>
     <div  class="contact--title text-3xl font-semibold not-italic mt-24">Deskripsikan Kebutuhan Anda, Kami Selalu Siap Membantu</div>
     <div  class="contact--title_isi font-semibold text-base not-italic mt-2 text-center mb-14">Kami menjamin bahwa semua data koresponden adalah bersifat RAHASIA dan tidak akan dipublikasikan.</div>
     
     </div>
</template>

<script>
export default {
    name: 'ContactView',
    components: {
    },
    data(){
      return{
  
      }
    },
    methods:{
  
    },
    mounted(){
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