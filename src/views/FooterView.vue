<template>
    <div class="footer w-full relative p-6"> 
        <div class="footer--box flex flex-col items-center justify-center">
            <div class="flex footer--logo mb-8"></div>
            <div class="flex"><p>Copyright 2011 - 2025 by PT. BAYUR JAYA - Jalan Raya Bayur No 72 Tangerang | <span><a href="tel:0215526610"> Call +62 21 552 6610 </a></span>  <span><a href="mailto:info@bayurjaya.co.id?subject=Mail from Our Site">| info@bayurjaya.co.id |</a></span> All Rights Reserved</p></div>
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
  }
}
</script>
<style lang="scss" scoped>
.footer{
    background-color: #0A2753;
    font-family: 'Cabin, Inter';
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