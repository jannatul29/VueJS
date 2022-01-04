<template>
    <div id="app">
      <nav class="container navbar navbar-expand-lg navbar-light bg-light" id="nav">
          <a class="navbar-brand" href="#">Logo Here</a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
             <div class="navbar-nav ms-auto">
                    <router-link to="/" class="nav-item nav-link">Offers</router-link>
                    <router-link to="/About" class="nav-item nav-link">Manage</router-link>
                    <router-link to="#" class="nav-link">Experience</router-link>
                    <router-link to="/About" class="nav-link">Marco Polo Club</router-link>
                </div>
            </div>
      </nav>
      <section id="featured-services" class="featured-services">
            <div class="container">
                <div class="row no-gutters" id="r1">
                    <div class="col-lg-11 col-md-6">
                      <div style="background-color: gainsboro;">
                        <span class="fw-bold">2 latest updates </span> View the latest COVID-19 travel restrictions, quarentine requirenments and more
                      </div>
                    </div>
                  </div>
                  <div class="row no-gutters" style="width: 1450px; text-align: left; height: 90px;">
                    <div class="col-lg-11 col-md-6" >
                      <div style="padding: 30px 0px 10px 0px">
                        <span style="font-size: 30px; font-weight: normal;">Ready for your next trip? Book with us now. </span>
                      </div>
                    </div>
                </div>
                <div class="row no-gutters" id="r1">
                    <div class="col-lg-7 col-md-6">
                        <div class="row no-gutters">
                            <div class="col-lg-12 col-md-6">
                                <div class="card" id="c1">
                                    <div class="row no-gutters">
                                        <div class="col-lg-6 col-md-6 p-0">
                                            <div>
                                                Flights
                                            </div>
                                        </div>
                                    </div>
                                     <hr>
                                     <div class="row no-gutters">
                                        <div class="col-lg-6 col-md-6 p-0">
                                            <div>
                                                <a  href="#" id="a1">Rendom flights</a><span id="s1"></span><a  href="#" id="a1">Multi-city/stopover</a>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="row no-gutters" >
                                        <div class="col-lg-3 col-md-6 p-0" id="col1">
                                            <div class="card btn btn-info" type="button" id="c2" data-bs-toggle="modal" data-bs-target="#myModal">
                                                <!-- <button type="button" class="btn btn-info">Info</button> -->
                                                <p>Leaving from</p>
                                                <p id="p1">{{ ita }}</p>
                                                <span id="p2">{{ cty }}</span>
                                            </div>
                                        </div>
                                        <div class="col-lg-3 col-md-6 p-0" id="col1">
                                            <div class="card btn btn-info" type="button" id="c2" data-bs-toggle="modal" data-bs-target="#myModal1">
                                                <!-- <button type="button" class="btn btn-info">Info</button> -->
                                                 <p>Going to</p>
                                                 <p id="p1">{{ ita1 }}</p>
                                                <span id="p2">{{ cty1 }}</span>
                                            </div>
                                        </div>
                                        <div class="col-lg-3 col-md-6 p-0" id="col1">
                                            <div class="card btn btn-info" type="button" id="c2" data-bs-toggle="modal" data-bs-target="#myModal2">
                                             <!-- <button type="button" class="btn btn-info">Info</button> -->
                                                <span>Departing on</span>
                                                <span id="p2">{{ dates.in }}</span>
                                                <hr>
                                                <!-- <HotelDatePicker /> -->
                                                <span>Returning on</span>
                                                <span id="p2">{{ dates.out }}</span>
                                            </div>
                                        </div>
                                        <div class="col-lg-3 col-md-6 p-0" id="col1">
                                            <div class="btn btn-info" type="button" id="c3">
                                            </div>
                                        </div>
                                    </div>
                                    <div class="row no-gutters">
                                        <div class="col-lg-6 col-md-6 p-0">
                                            <div>
                                                <a  href="#" id="a1">Return<i class="bi bi-chevron-down"></i></a><span id="s1"></span><a  href="#" id="a1">Economy, 1 Audlt<i class="bi bi-chevron-down"></i></a>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="row no-gutters" style="padding: 20px 0px 0px 0px;">
                            <div class="col-lg-12 col-md-6">
                                <div id="d1">
                                    <div class="row no-gutters" id="r3">
                                        <div class="col-lg-3 col-md-6 p-0">
                                          <div class="icon-box" id="i1">

                                          </div>
                                        </div>
                                        <div class="col-lg-3 col-md-6 p-0">
                                          <div class="icon-box" id="i1">
                                            <br><br>
                                          </div>
                                        </div>
                                        <div class="col-lg-3 col-md-6 p-0">
                                          <div class="icon-box" id="i1">
                                            <br><br>
                                          </div>
                                        </div>
                                        <div class="col-lg-3 col-md-6 p-0">
                                          <div class="icon-box" id="i1">
                                            <br><br>
                                          </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-5 col-md-6">
                        <!-- <div class="icon-box" style="background-image: url(assets/img/slide/slide-1.jpg);"> -->
                          <img src="assets/img/slide/slide-1.jpg" height="500" width="462">
                        <!-- </div> -->
                    </div>
                </div>
            </div>
        </section>


          <div class="modal" id="myModal">
  <div class="modal-dialog">
    <div class="modal-content">

      <!-- Modal Header -->
      <div class="modal-header">
        <h4 class="modal-title">Select a departure city</h4>
        <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
      </div>

      <!-- Modal body -->
      <div class="modal-body">
        <div>
      <input
        type="text"
        class="form-control"
        placeholder="Leaving from"
        v-model="uname"
        @input="getUser"
      />
    </div>
    <div>
     <ul class="">
          <p @click="setState(user)" v-for="user in users" :key="user.n">
            {{ user.name }}
          </p>
        </ul>  
    </div>

  </div>
      </div>

    </div>
  </div>
  
<div class="modal" id="myModal1">
  <div class="modal-dialog">
    <div class="modal-content">

      <!-- Modal Header -->
      <div class="modal-header">
        <h4 class="modal-title">Select a departure city</h4>
        <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
      </div>

      <!-- Modal body -->
      <div class="modal-body">
        <div>
      <input
        type="text"
        class="form-control"
        placeholder="Leaving from"
        v-model="uname1"
        @input="getUser1"
      />
    </div>
    <div>
     <ul class="">
          <p @click="setState1(user1)" v-for="user1 in users1" :key="user1.n">
            {{ user1.name }}
          </p>
        </ul>  
    </div>
  </div>
      </div>

    </div>
  </div>


        <div class="modal" id="myModal2">
          <div class="modal-dialog">
            <div class="modal-content">
              <div class="modal-header">
                 <h4 class="modal-title">Modal Heading</h4>
                <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
              </div>
              <div class="modal-body">
                <HotelDatePicker @check-in-changed="checkIn" @check-out-changed="checkOut"/>
              </div>
            </div>
          </div>
        </div>

      <router-view/>
    </div>
</template>
<script>
import axios from 'axios'
import HotelDatePicker from 'vue-hotel-datepicker'
import 'vue-hotel-datepicker/dist/vueHotelDatepicker.css'
// import Datepicker from 'vuejs-datepicker'
export default {
  name: 'App',
  components: {
    HotelDatePicker
  },
  // components: {
  //   Datepicker
  // },
  data: function() {
    return {
      uname: "",
      cty: "Dhaka",
      ita: "DAC",
      users: [],
      uname1: "",
      cty1: "Dhaka",
      ita1: "DAC",
      users1: [],
      dates: {
        in: null,
        out: null
      }

    }
  },
  methods: {
    getUser() {
        console.log(this.uname)
        axios.get("https://api.sharetrip.net/api/v1/flight/search/airport?name=" + this.uname)
        .then(res => {
                //console.log("axios")
                console.log(res.data)
                this.users = res.data.response;
                
        })
        .catch((err) => {
            console.log(err)
        });
    },

    setState(user){
        console.log(user)
        this.uname = user.name
        this.cty = user.city
        this.ita = user.iata
        this.users = []
    },

    getUser1() {
        console.log(this.uname1)
        axios.get("https://api.sharetrip.net/api/v1/flight/search/airport?name=" + this.uname1)
        .then(res => {
                //console.log("axios")
                console.log(res.data)
                this.users1 = res.data.response;
                
        })
        .catch((err) => {
            console.log(err)
        });
    },

    setState1(user1){
        console.log(user1)
        this.uname1 = user1.name
        this.cty1 = user1.city
        this.ita1 = user1.iata
        this.users1 = []
    },
    checkIn(val) {
      //console.log(val.toLocaleString().slice(0, 10).replaceAll("/", "-"));
      var d = val.toLocaleString().split(",");
      console.log(d[0].replaceAll("/", "-"));
      console.log(val.toString().slice(4,14));
      this.dates.in = val.toString().slice(4,14);
      //this.dates.in = val.toISOString().slice(0, 10);
    },
    checkOut(val) {
      console.log(val.toISOString().slice(0, 10));
      this.dates.out = val.toString().slice(4,14);
      //this.dates.out = val.toISOString().slice(0, 10);
    }
    
  }
}
</script>
<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 0px;
  }
  #nav {
    padding: 30px;
  }
  #nav a {
    font-weight: bold;
    color: #2c3e50;
  }
  #nav a.router-link-exact-active {
    color: #42b983;
  }
  #r1 {
    width: 1450px;
  }
  #c1 {
    background-color: white;
    border-style: groove;
    padding: 20px;
  }
  #a1 {
    color: darkcyan;
    text-decoration: none;
  }
  #s1 {
    padding: 0px 20px 0px 0px;
  }
  #c2 {
    background-color: rgb(255, 255, 255);
    height: 154px;
  }
  #c3 {
    background-repeat: no-repeat;
    height: 154px; width: 196px;
  }
  #col1 {
    border-style: outset;
  }
  #p1 {
    font-size: 30px;
    font-weight: bold;
  }
  #p2 {
    font-size: 20px;
    font-weight: bold;
  }
  #d1 {
    background-color: white;
    padding: 10px;
  }
  #r3 {
    padding: 0px 0px 0px 0px;
    border-radius: 5px;
  }
  #i1 {
    background-color: rgb(83, 17, 17);
  }
</style>
