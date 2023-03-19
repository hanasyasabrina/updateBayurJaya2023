<template>
  <div class="about insider bg-white w-full h-full flex justify-center items-center flex-col"> 
      <!-- mulai dari sini -->
      <div class="flex justify-center items-center flex-col">
        <div class="insider--catalog2 mb-8 text-3xl">Sewa Mesin Boring HDD</div>
        <div class="insider--download insider--catalog5">CALL FOR RENTAL</div>
      </div>
      <div class="insider__box my-20 flex items-center justify-center">
          <img :src="require(`../assets/gallery/boringHDD/boringhdd.png`)"/>
      </div> 
      <div class="mt-20 flex flex-col items-center justify-center insider--catalog4">
        <div class="insider__story--text gap-4 insider--catalog3">
          <p>Kami menyediakan jasa pelayanan sewa mesin bor HDD yang dapat digunakan untuk pemasangan jaringan kabel optik / listrik, pipa HDPE atau PE dan lainnya. Dengan menggunakan mesin bor HDD ini maka tidak perlu dilakukan penggalian jalan atau bangunan yang akan dilewati jalur instalasi kabel/pipa, sehingga dapat menghemat waktu dan biaya karena tidak memerlukan banyak tenaga manusia untuk melakukan penggalian sebagaimana pemasangan instalasi jaringan kabel/pipa secara manual.</p>
          <p>Kami akan memberikan dukungan penuh dengan tenaga ahli dan peralatan yang telah dilengkapi dengan Surat Ijin Operator (SIO) dan Surat Ijin Laik Operasi (SILO) dari Instansi terkait.</p>
        </div>
      </div>
      <div class="insider__box insider__box--image my-20 flex items-center justify-center">
          <img :src="require(`../assets/gallery/boringHDD/boringhdd.png`)"/>
      </div> 

  </div>
</template>
<script>
export default {
  name: 'AboutView',
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
.insider{
  font-family: 'Montserrat, Inter';
  background-color: white;
  margin-top: -1px;

  &--catalog{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: -120px;
      left: -180px;
      background-image: url('../assets/ornament/insider.png');
      background-repeat: no-repeat;
      background-size: contain;
      width: 150px;
      height: 120px;
    }
  }

    &--catalog2{
    position: relative;
    &:before{
      content: "";
      position: absolute;
      top: 200px;
      left: -520px;
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
      top: 260px;
      left: 1063px;
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
      top: 1385px;
      left: -380px;
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
    font-family: 'Inter';
    font-weight: 700;
    font-size: 18px;
    border-radius: 4px;
    // max-width: 165px;
    cursor: pointer;
    &:hover{
      background-color: #4B0E0E;
    }
  }
  &__story{
    &--text{
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
      // flex: 1 1 0;
      width: 100%;
      height: 100%;
      // background-position: center;
      // background-size: contain;
      // background-repeat: no-repeat;
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
