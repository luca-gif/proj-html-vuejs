<template>
  <div>
    <footer class="p-5">
      <div class="row">

        <div class="col-4">
          <img src="../assets/img/medical_logo_1x_dark.png" alt="Avada logo">
          <p class="py-3 text-muted">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium dolemue launti totam aperiam, eaque ipsa quae abillo. Invente veriatis et quasi architecto beatae luptatem accusantium, remaperiamsiat. Voluptatem accusest etsium doloremque laudaien. Lorem ipsum sits dolores ets unser.</p>
        <div class="border mb-1"></div>
        <p class="text-muted">LEARN MORE ABOUT US</p>
          <div class="social d-flex mb-4">
            <i class="fa-brands fa-facebook-f facebook social-icon"></i>
            <i class="fa-brands fa-twitter twitter social-icon"></i>
            <i class="fa-brands fa-instagram instagram social-icon"></i>
            <i class="fa-brands fa-youtube youtube instagram social-icon"></i>
          </div>
        </div>

        <div class="col-4 contact">
          <div>CONTACT INFORMATION</div>
          <div class="border-blu my-3"></div>
          <div class="py-2 text-muted">
            <i class="fa-solid fa-location-dot"></i> 121 King Street, London United Kingdom 
          </div>
           <div class="text-muted">
            <i class="fa-solid fa-phone-flip"></i> 1.800.458.556
           </div>
        </div>
        
        <div class="col-4 medical-department">
          <div>MEDICAL DEPARTMENT</div>
          <div class="border-blu my-3"></div>
          <ul>
            <li v-for="(list,index) in footerList" :key="`footer${index}`" class="d-flex align-items-center">
            <i class="fa-solid fa-circle-check"></i> {{list.name}}
            </li>
          </ul>

          <div class="lm-btn">
            VIEW OUR DEPARTMENTS
          </div>
        </div>
      </div>
    </footer>

    <div class="copyright d-flex align-items-center px-5 text-muted">
      <div>© Copyright 2012 - 2022 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterComp',
  props:{
    footerList: Array
  }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/var';

  .contact i{
    color: $primary-color;
    width: 20px;
    margin-right: 5px;
    text-align: center;
  }

  .medical-department i{
    color: $primary-color;
    font-size: 20px;
    margin-right: 5px;
    }

  .border-blu{
    background-color: $primary-color;
    height: 2px;
    width: 40px;
  }

  .lm-btn{
    background-color: #fff;
    border: 1px solid black;
    width: 260px;
    text-align: center;
    margin-top: 30px;
    
    &:hover{
      background-color: $primary-color;
      color: #fff;
      border: transparent;
    }
  }

  .copyright{
    background-color: #f7f7f7;
    height: 50px;
    font-size: 12px;
  }

</style>