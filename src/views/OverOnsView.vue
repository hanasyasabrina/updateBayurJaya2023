<template>
  <div class="over-ons px-4 xl:px-0 bg-white w-full h-full flex justify-center items-center flex-col"> 
      <!-- mulai dari sini -->
      <div class="over-ons--catalog3 flex justify-center items-center flex-col">
        <div class="over-ons--title text-center mb-8 text-3xl">Sewa Mesin Boring HDD</div>
        <div class="over-ons--download">CALL FOR RENTAL</div>
      </div>
      <div class="over-ons--catalog mt-20 flex flex-col items-center justify-center">
        <div>VIDEO</div>
      </div>
      <div class="over-ons__box my-20 flex items-center justify-center">
        <div class="over-ons--catalog4"></div>
        <div class="over-ons--catalog5"></div> 
        <div class="over-ons__story--text text-base gap-4">
          <p>Kami menyediakan jasa pelayanan sewa mesin bor HDD yang dapat digunakan untuk pemasangan jaringan kabel optik / listrik, pipa HDPE atau PE dan lainnya. Dengan menggunakan mesin bor HDD ini maka tidak perlu dilakukan penggalian jalan atau bangunan yang akan dilewati jalur instalasi kabel/pipa, sehingga dapat menghemat waktu dan biaya karena tidak memerlukan banyak tenaga manusia untuk melakukan penggalian sebagaimana pemasangan instalasi jaringan kabel/pipa secara manual.</p>
          <p>Kami akan memberikan dukungan penuh dengan tenaga ahli dan peralatan yang telah dilengkapi dengan Surat Ijin Operator (SIO) dan Surat Ijin Laik Operasi (SILO) dari Instansi terkait.</p>
        </div>
        <div class="over-ons__box--image flex">
          <img :src="require(`../assets/over-ons-hdd.png`)"/>
        </div>
      </div>

  </div>
</template>
<script>
export default {
  name: 'OverOnsView',
  components: {
    // HelloWorld
  },
  data(){
    return{
      dataFoto:[
        {
          url:"Radar2.jpeg",
          tag: "mekanikal",
        },
        {
          url:"Thaha.jpeg",
          tag: "sipil",
        },
        {
          url:"Radar6.jpeg",
          tag: "sipil",
        },
        {
          url:"rtil3.jpeg",
          tag: "sipil",
        },
        {
          url:"sqfl2.jpeg",
          tag: "sipil",
        },
        {
          url:"Thaha3.jpeg",
          tag: "sipil",
        }
      ]
    }
  },
  methods:{

  },
  mounted(){
  }
}
</script>
<style lang="scss" scoped>
@mixin smartphone {
    @media (max-width: 599px) { @content; }
  }
.over-ons{
  font-family: 'Montserrat, Inter';
  background-color: white;
  margin-top: -1px;

  &--title{
    font-family: 'Montserrat';
  }

  &--catalog{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: -70px;
      left: -650px;
      background-image: url('../assets/ornament/insider2.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 50px;
      height: 350px;
    }
  }

    &--catalog3{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: 620px;
      left: 750px;
      background-image: url('../assets/ornament/insider3.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 154px;
      height: 360px;
      }
    }

    &--catalog4{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: 490px;
      left: -40px;
      background-image: url('../assets/ornament/insider4.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 32px;
      height: 32px;
      }
    }

    &--catalog5{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: 500px;
      left: -30px;
      background-image: url('../assets/ornament/insider5.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 61.98px;
      height: 61.98px;
      transform: rotate(10.5deg);
      }
    }

  &--download{
    padding: 20px 64px;
    background-color: #0E1C4B;
    transition: 0.5s;
    color: white;
    font-family: 'Cabin';
    font-weight: 700;
    font-size: 18px;
    border-radius: 4px;
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
  &__story{
    &--text{
      font-family: 'Cabin';
      max-width: 1000px;
      p{
        margin-bottom: 12px;
      }
    }
  }
  &__box{
    flex-wrap: wrap;
    width: 100%;
    max-width: 1000px;


    &--image{
      width: 80%;
      height: 100%;
      &:hover{
        transform: scale(1.2);
      }
    }

  }
  
}

video{
  position: absolute;
  width: 1158px;
  height: 588px;
  left: 141px;
  top: 460px;

  background: #D9D9D9;
}
</style>
