<template>
  <div>
    
    <header>

      <nav class="d-flex justify-content-between align-items-center">

        <div class="nav-logo">
          <img src="../assets/img/medical_logo_1x_light.png" alt="">
        </div>
        
          <ul class="d-flex align-items-center">

            <li @click="list.isActive = !list.isActive" v-for="list in headerList" :key="list"><a :class="{'active' : list.isActive}" href="#">{{list.name}}</a></li>
            
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

    </header>
  </div>
</template>

<script>
export default {
  name: 'HeaderComp',

  props:{
    headerList: Array
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

.active{
  color: $primary-color;
  font-weight: 900;
  text-decoration:overline;
}

</style>