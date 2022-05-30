<template>
  <div>
    
    <header>

      <nav class="d-flex justify-content-between align-items-center">

        <div class="nav-logo">
          <img src="../assets/img/medical_logo_1x_light.png" alt="">
        </div>
        
          <ul class="d-flex align-items-center">

            <li @click="currentIndex = index" v-for="(list,index) in headerList" :key="`list${index}`"><a :class="{'active' : currentIndex === index}" href="#">{{list.name}}</a></li>
            
            <li class="lm-btn"><a href="#">Make Appointment</a></li>
          </ul>
        
      </nav>

      <div class="header-bottom container m-auto d-flex align-items-center">
        <div class="header-container">
        <h1>Caring <span>For Life</span></h1>
        <p>Kind words can be short and easy to speak, but their echoes are truly endless. Avada Health focuses on you as if it was our own family.</p>
        <span class="lm-btn">Learn More</span>
        </div>
      </div>

      <div v-show="showHours" class="office-hours text-center">
        <h5 class="hours-title">OFFICE HOURS</h5>
        <div class="line"></div>

          <div class="hours text-start">
            <strong><span>Monday - Friday</span> <span class="float-end">8:00 - 5:00</span></strong> <br>
            <strong><span>Saturday</span>	<span class="float-end">8:00 - 5:00</span></strong> <br>
            <strong><span>Sunday</span> <span class="float-end">8:00 - 5:00</span></strong>
          </div>

        <div class="phone"> +44(0) 1865 339665</div>
      </div>

      
      <a href="#">
        <div class="anchor">
          <i class="fa-solid fa-angle-up"></i>
        </div>
      </a>

    </header>
  </div>
</template>

<script>
export default {
  name: 'HeaderComp',
  data(){
    return{
      showHours: false,
      currentIndex: 0,
    }
  },

  props:{
    headerList: Array
  },

  methods:{
    setShow() {
      setTimeout(() => {
        this.showHours = true;
      }, 1000);
    }
  },

   mounted(){
      this.setShow()
  }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/var';

header{
  background-image: url(../assets/img/header-image-homepage.jpg);
  background-size: cover;
  color: #fff;
  height: 750px;
  font-family: 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  position: relative;
  top: 0;
}

nav{
  height: 100px;
  padding: 0px 40px;

    ul{
      margin: 0;
    }

    ul li{
    margin-left: 30px;
    text-transform: uppercase;
    font-size: 13px;

    a{
      color: #fff
    }
  } 
}

.lm-btn:hover{
  background-color: #327ec7;
  transition: all .4s;
}

.header-container{
  width: 60%;
  height: 250px;
}

.header-bottom{
  height: calc(600px - 140px);
  font-size: 1.1rem;

  h1{
    font-size: 60px;
  }

  h1 span{
    color: $primary-color;
  }

  p{
    padding: 15px 0;
  }

}

.office-hours{
  width: 350px;
  height: 350px;
  background-color: rgba($color: $primary-color, $alpha: .4);
  padding: 40px 30px;
  position: absolute;
  right: 220px;
  bottom: 200px;

  .line{
    height: 4px;
    width: 100%;
    background-color: $primary-color;
  }

  .hours{
    padding: 35px 0;
  }

  strong{
    display: block;
    height: 30px;
  }

  
}

.anchor{
  position: fixed;
  bottom: 0;
  right: 70px;
  height: 35px;
  width: 50px;
  background-color: #484848;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 5px 5px 0 0;
  cursor: pointer;
  transition: all .6s;

  &:hover{
    background-color: $primary-color;
  }

  i{
    color: #fff;
  }
}

.active{
  color: $primary-color;
  font-weight: 900;
  text-decoration:overline;
}

</style>