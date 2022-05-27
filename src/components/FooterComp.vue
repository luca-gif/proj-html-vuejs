<template>
  <div>
    <footer class="p-5">
      <div class="row">

        <div class="col-4">
          <img src="../assets/img/medical_logo_1x_dark.png" alt="">
          <p class="py-3 text-muted">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium dolemue launti totam aperiam, eaque ipsa quae abillo. Invente veriatis et quasi architecto beatae luptatem accusantium, remaperiamsiat. Voluptatem accusest etsium doloremque laudaien. Lorem ipsum sits dolores ets unser.</p>
        <div class="border mb-1"></div>
        <p class="text-muted">LEARN MORE ABOUT US</p>
        </div>

        <div class="col-4">
          <div>CONTACT INFORMATION</div>
          <div class="border-blu my-3"></div>
          <div class="text-muted">
            121 King Street, London United Kingdom 
          </div>
           <div class="text-muted">
            1.800.458.556
           </div>
          
        </div>
        
        <div class="col-4">
          <div>MEDICAL DEPARTMENT</div>
          <div class="border-blu my-3"></div>
          <ul>
            <li><a href="#">Cardioligy</a></li>
            <li><a href="#">Pedriatics</a></li>
            <li><a href="#">Diabetes Care</a></li>
            <li><a href="#">Pre-natel Care</a></li>
            <li><a href="#">Ultrasound Echocardiogram</a></li>
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
}
</script>

<style lang="scss" scoped>

@import '../assets/style/var';

  .border-blu{
    background-color: $primary-color;
    height: 1.5px;
    width: 40px;
  }

  .lm-btn{
    background-color: #fff;
    border: 1px solid black;
    width: 250px;
    text-align: center;
    cursor: pointer;
    margin-top: 30px;
  }

  a{
    color: black;
  }

  .copyright{
    background-color: #f7f7f7;
    height: 50px;
    font-size: 12px;
  }

</style>