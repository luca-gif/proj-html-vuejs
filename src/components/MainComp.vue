<template>
  <div>

    <!-- Welcome To Avada  Health-->
    <div class="container">

      <section class="welcome text-center my-5">

        <h2>Welcome to Avada Health</h2>
        <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium <br> doloremque laudantium, totam
          rem aperiam, eaque ipsa quae ab illo</p>


        <div class="row my-5">

          <div class="col-3 text-center">
            <img src="../assets/img/icon-1.png" alt="">
            <p class="">SAME DAY APPOINTMENTS</p>
            <p class="text-muted">Sed ut perspiciatis unde omnis iste natus error sit voluptam accusantim</p>
          </div>

          <div class="col-3 text-center">
            <img src="../assets/img/icon-2.png" alt="">
            <p>WORLD CLASS FACILITIES</p>
            <p class="text-muted">Sed ut perspiciatis unde omnis iste natus error sit voluptam accusantim</p>
          </div>

          <div class="col-3 text-center">
            <img src="../assets/img/icon-3.png" alt="">
            <p>EXPERT DOCTORS</p>
            <p class="text-muted">Sed ut perspiciatis unde omnis iste natus error sit voluptam accusantim</p>
          </div>

          <div class="col-3 text-center">
            <img src="../assets/img/icon-4.png" alt="">
            <p>COMPLEMENTARY THERAPIES</p>
            <p class="text-muted">Sed ut perspiciatis unde omnis iste natus error sit voluptam accusantim</p>
          </div>

        </div>

      </section>

    </div>

    <!-- Meet our doctors -->

    <section  class="meet-our-doctors text-center py-5">
      <div class="doctors-text container">
        <div class="container">

          <img src="../assets/img/icon-5.png" alt="">
          <h2>MEET OUR DOCTORS</h2>
          <div class="border w-50 m-auto my-4"></div>
          <p>
            Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem
            aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae
          </p>
        </div>
      </div>

      <div class="container">

        <div class="row py-4">
          <div v-for="doctor in doctors" :key="doctor.id" class="col-4 card">
            <img :src= "doctor.image" :alt="doctor.nome">
            <div class="card-text">
              <h6 class="pt-3">{{doctor.nome}}</h6>
              <h6>{{doctor.professione}}</h6>
              <p class="pt-3 text-muted">{{doctor.descrizione}}</p>
              <div class="social d-flex mb-4">
                <i class="fa-brands fa-facebook-f facebook social-icon"></i>
                <i class="fa-brands fa-twitter twitter social-icon"></i>
                <i class="fa-brands fa-instagram instagram social-icon"></i>
              </div>
            </div>
          </div>
        </div>

      </div>
    </section>

    <!-- Our Healt Services -->

    <section class="services py-5">
      <div class="container">
        <div class="mini-container">

          <div class="services-text">
            <img src="../assets/img/icon-6.png" alt="">
            <h2>OUR HEALTH SERVICES</h2>
            <div class="border w-50 m-auto my-4"></div>
            <p>
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam
              rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae
            </p>
          </div>

        </div>

        <div class="row my-5 text-center">

          <div class="col-4">
            <img src="../assets/img/icon-14.png" alt="">
            <p>REHABILITATION CENTER</p>
            <p class="text-muted">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium
              voluptatum deleniti atque corrupti quos dolores et quas </p>
          </div>

          <div class="col-4">
            <img src="../assets/img/icon-15.png" alt="">
            <p>DENTAL IMPLANTS</p>
            <p class="text-muted">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium
              voluptatum deleniti atque corrupti quos dolores et quas </p>
          </div>

          <div class="col-4">
            <img src="../assets/img/icon-16.png" alt="">
            <p>MEDICINE RESEARCH</p>
            <p class="text-muted">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium
              voluptatum deleniti atque corrupti quos dolores et quas </p>
          </div>

        </div>
        <div class="row my-5 text-center">

          <div class="col-4">
            <img src="../assets/img/icon-11.png" alt="">
            <p>BLOOD BANK</p>
            <p class="text-muted">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium
              voluptatum deleniti atque corrupti quos dolores et quas </p>
          </div>

          <div class="col-4">
            <img src="../assets/img/icon-12.png" alt="">
            <p>PHARMACEUTICAL ADVICE</p>
            <p class="text-muted">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium
              voluptatum deleniti atque corrupti quos dolores et quas </p>
          </div>

          <div class="col-4">
            <img src="../assets/img/icon-13.png" alt="">
            <p>MEDICAL COUNSELING</p>
            <p class="text-muted">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium
              voluptatum deleniti atque corrupti quos dolores et quas </p>
          </div>

        </div>

      </div>
    </section>

    <!-- Tour Facilities -->

    <section class="tour-facilities text-white">
      <div class="container h-100 d-flex align-items-center">
        <div class="mini-container">

          <img src="../assets/img/icon-7.png" alt="">
          <h2 class="my-3">TOUR OUR FACILITIES</h2>
          <div class="border w-50 m-auto my-4"></div>
          <p class="my-3">
            Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem
            aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae
          </p>
          <img src="../assets/img/play-icon.png" alt="">

        </div>
      </div>

    </section>

    <div class="skills text-white">
      <div class="row text-center">

        <div class="first-skill col-4 py-5">
          <h6>Emergency Care</h6>
          <img src="../assets/img/wave-divider.png" alt="">
          <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem
            aperiam, eaque</p>
          <span class="lm-btn">Learn More</span>
        </div>

        <div class="second-skill col-4 py-5">
          <h6>Emergency Care</h6>
          <img src="../assets/img/wave-divider.png" alt="">
          <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem
            aperiam, eaque</p>
          <span class="lm-btn">Learn More</span>
        </div>

        <div class="third-skill col-4 py-5">
          <h6>Emergency Care</h6>
          <img src="../assets/img/wave-divider.png" alt="">
          <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem
            aperiam, eaque</p>
          <span class="lm-btn">Learn More</span>
        </div>

      </div>
    </div>

    <!-- Make An Appointment -->

    <section class="appointment">
      <div class="container h-100 d-flex align-items-center text-white">
        <div class="mini-container">

          <h2 class="my-3">Make An Appointment</h2>
          <p class="my-3">
            Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem
            aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae
          </p>

          <form class="">
            <input @keyup.enter="apiSend()" type="text" v-model.trim="newAppointment.name" placeholder="Name*">
            <input @keyup.enter="apiSend()" type="email" v-model.trim="newAppointment.email" placeholder="Email*">
            <input @keyup.enter="apiSend()" type="text" v-model.trim="newAppointment.phone" placeholder="Phone Number">
            <input @keyup.enter="apiSend()" type="date" v-model.trim="newAppointment.date" placeholder="Appointment Date">
            <textarea v-model.trim="newAppointment.request" name="" cols="30" rows="3" placeholder="How can we help!?"></textarea>
            <div @click="apiSend()" class="lm-btn insert text-white">MAKE AN APPOINTMENT</div>
          </form>

        </div>
      </div>
    </section>

    <div class="banner d-flex justify-content-center align-items-center">

       <VueSlickCarousel class="w-75" :arrows="true" :dots="false" v-bind="settings">
      <div class="text-center"><img src="../assets/img/client-logos-1.png" alt=""></div>
      <div class="text-center"><img src="../assets/img/client-logos-3.png" alt=""></div>
      <div class="text-center"><img src="../assets/img/client-logos-2.png" alt=""></div>
      <div class="text-center"><img src="../assets/img/client-logos-4.png" alt=""></div>
      <div><img src="../assets/img/client-logos-2.png" alt=""></div>
    </VueSlickCarousel>

    </div>

    <!-- Ancora -->

      <anchorComp/>

  </div>
</template>

<script>

import axios from 'axios';
import 'vue-slick-carousel/dist/vue-slick-carousel.css';
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css';
import VueSlickCarousel from 'vue-slick-carousel';
import AnchorComp from './AnchorComp.vue';


export default {
  name: 'MainComp',
  components: { VueSlickCarousel,AnchorComp },

  data(){
      return{
        
        endpoint: 'http://localhost:3000/clienti',
        arrData: [],
        newAppointment: {
            name: '',
            email: '',
            phone: '',
            date: '',
            request: ''
        },

        settings: {
          "dots": false,
          "focusOnSelect": false,
          "infinite": true,
          "speed": 1000,
          "slidesToShow": 4,
          "slidesToScroll": 1,
          "touchThreshold": 5,
          "autoplay": true,
          "autoplaySpeed": 3000,
        }
    }
  },

  props:{
    doctors: Array
  },

    methods:{
    apiRequest(){
      axios.get(this.endpoint)
      .then((r) => {
        this.arrData = r.data
        console.log(this.arrData)
      })
    },

    apiSend(){
      axios.post(this.endpoint, this.newAppointment)
      .then((r) => {
        this.newAppointment = {
            name: '',
            email: '',
            phone: '',
            date: ''
        }
        
        console.log(r.data)
        this.apiRequest()
      })
    }
  },
}
</script>

<style lang="scss" scoped>
@import '../assets/style/var';

p {
  line-height: 2rem;
}

.col-3 {
  p {
    font-size: 13px;
  }
}

.meet-our-doctors {
  background-color: #f7f7f7;

  img{
    transition: all .5s;  
  
    &:hover{
      transform: scale(105%);
      box-shadow: 0 0 5px gray ;
    }
  }

  .col-center {
    padding: 0 20px;
    margin: 0 30px;
  }

  .card {
    padding: 0;
    border: 0;
    margin: 0 10px;
    border-radius: 0;
    width: calc(100% / 3 - 20px);
    text-align: left;
    overflow: visible;

    p {
      font-size: 13px;
    }

    .card-text {
      padding: 0 35px;
    }
  }
}

.services {

  .col-4>img {
    padding: 20px 0;
  }
}

.tour-facilities {
  background-image: url(../assets/img/paralax-bg-tour-facilities.jpg);
  background-position: center;
  background-size: cover;
  height: 550px;

  img {
    width: 50px;
  }
}

.first-skill {
  background-color: #3aafbf;

  .lm-btn {
    background-color: #3aafbf;
    border: white 2px solid;
    cursor: pointer;
  }
}

.second-skill {
  background-color: #3597c3;

  .lm-btn {
    background-color: #3597c3;
    border: white 2px solid;
    cursor: pointer;
  }
}

.third-skill {
  background-color: #327ec7;

  .lm-btn {
    background-color: #327ec7;
    border: white 2px solid;
    cursor: pointer;
  }
}

.appointment {
  height: 700px;
  background-image: url(../assets/img/make-an-appointment.jpg);
  background-position: center;
  background-size: cover;
}

form {
  input {
    width: calc(50% - 20px);
    margin: 10px;
  }

  textarea {
    width: calc(100% - 20px);
    margin: 10px;
  }

  input,
  textarea {
    background-color: transparent;
    color: #fff;
    border: 1px solid #fff;
    padding: 6px 15px;

    &:focus {
      outline: none;
    }

    &::placeholder {
      color: #fff;
      font-size: 10px;
    }
  }

  .insert {
    width: calc(100% - 20px);
    margin-left: 10px;
    font-weight: bold;
    border: transparent;
  }
}

.banner {
  background-image: linear-gradient(to right, #3bafbf, #327fc7);
  height: 300px;


  img {
    cursor: pointer;
  }
}
</style>