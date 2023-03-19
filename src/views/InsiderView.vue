<template>
    <div class="about insider bg-white px-4 xl:px-0 w-full h-full flex justify-center items-center flex-col"> 
        <!-- mulai dari sini -->
        <div class="flex justify-center items-center flex-col">
          <div class="insider--title text-center mb-8 text-3xl">Get Our Catalog</div>
          <div class="insider--download">DOWNLOAD COMPANY PROFILE</div>
        </div>
        <div class="insider--catalog mt-20 flex flex-col items-center justify-center">
          <div class="insider--title mb-8 text-3xl">Our Story</div>
          <div class="insider__story--text text-base gap-4">
            <p>Berawal dari keinginan untuk menjadi seorang pengusaha agar dapat membuka lapangan pekerjaan untuk orang lain, maka pada tanggal 8 Mei 2008 bapak Sungkono bin Somo Karyono mendirikan perusahaan di Tangerang dan disahkan dengan akta notaris Herry Sosiawan, S.H no. 104 dengan nama </p>
            <p>CV. Bayur Jaya yang bergerak dibidang usaha Jasa Konstruksi, Pengadaan Barang & Jasa dan Perdagangan Umum. Dengan ketekunan disertai kerja keras dan komitmen beliau yang tinggi maka pada tanggal 18 November 2011 CV. Bayur Jaya ditingkatkan statusnya menjadi  PT. Bayur Jaya dan disahkan dengan akta notaris Herry Sosiawan, S.H no. 152. Berbekal dengan ijin usaha dan kepercayaan yang diberikan oleh klien dan partner, kami terus berupaya meningkatkan kualitas, efektifitas dan efisiensi serta meningkatkan standar pelayanan kerja. Seiring dengan kemajuan teknologi dan tuntutan pelanggan serta persaingan yang sangat kompetitif dalam perusahaan jasa konstruksi kami menerapkan Standar Mutu ISO sejak tahun 2011.</p>
            <p>Saat ini kami terus meningkatkan dan mengembangkan bidang usaha dengan menambah peralatan kerja sebagai penunjang project yang dipercayakan ke kami serta peningkatan SDM yang berkualitas dan berpengalaman dalam bidangnya masing-masing dan telah tersertifikasi. Atas kepercayaan yang telah diberikan kepada kami di tahun-tahun sebelumnya tentunya menjadi tantangan berat yang harus kami jaga dan tingkatkan untuk dijadikan acuan dalam mewujudkan tujuan kami, yaitu “Menjadi perusahaan Jasa Konstruksi Nasional yang berintegritas dan kredibel berlandaskan layanan dan kualitas hasil pekerjaan yang prima dengan dukungan team kerja yang solid”.</p>
          </div>
        </div>
        <div class="insider__box my-20 flex items-center justify-center">
          <div class="insider__box--image flex" v-for="(index, key) in dataFoto" :key="key">
            <img :src="require(`../assets/gallery/runwayGardu/${index.url}`)"/>
          </div>
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
      console.log("ini insider")
    }
  }
  </script>
  <style lang="scss" scoped>
  @mixin smartphone {
    @media (max-width: 599px) { @content; }
  }
  .insider{
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
        top: -120px;
        left: -180px;
        background-image: url('../assets/ornament/insider.png');
        background-repeat: no-repeat;
        background-size: contain;
        width: 150px;
        height: 120px;
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
        // flex: 1 1 0;
        width: 30%;
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
  </style>