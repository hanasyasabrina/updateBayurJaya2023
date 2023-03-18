<template>
    <div class="footer w-full relative p-6"> 
        <div class="footer--box flex flex-col items-center justify-center">
            <div class="flex footer--logo mb-8"></div>
            <div class="flex">Copyright 2011 - 2023 by PT. BAYUR JAYA - Jalan Raya Bayur No 72 Tangerang Phone +6221 552 6610 | info@bayurjaya.co.id | All Rights Reserved</div>
        </div>
        <!-- mulai dari sini -->
    </div>
</template>
<script>
export default {
  name: 'FooterView',
  components: {
    // HelloWorld
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
.footer{
    background-color: #0A2753;
    font-family: 'Montserrat, Inter';
    // position: absolute;
    &--box{
        color: white;
        background-color: #0A2753;
    }
    &--logo{
        background-image: url('../assets/logo-footer.png');
        background-repeat: no-repeat;
        background-position: center;
        background-size: contain;
        width: 280px;
        height: 72px;
    }
}
</style>