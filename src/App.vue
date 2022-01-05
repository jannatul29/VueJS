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
      <section id="featured-services" class="featured-services section-bg">


      
      <div class="container">
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6" style="background-color: gainsboro;">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span class="fw-bold">2 latest updates </span> View the latest COVID-19 travel restrictions, quarentine requirenments and more
          </div>
        </div>
        <!-- 1st row end-->
        <br>
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6">
            <div class="icon-box">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span style="font-size: 30px; font-weight: normal;">Ready for your next trip? Book with us now. </span>
            </div>
          </div>
        </div>
        <!-- 1st row end-->
        <br>
<div class="row no-gutters">
    <div class="col-lg-8 col-md-6">

      <div class="row no-gutters">
        <div class="col-lg-12 col-md-6">
            <div>
                <p>Flights</p>
            </div>
        </div>
    </div>
    <div class="row no-gutters">
      <div class="col-lg-3 col-md-6">
          <div>
            <a  href="#" id="a1">Rendom flights</a>
          </div>
      </div>
      <div class="col-lg-4 col-md-6">
        <div>
          <a  href="#" id="a1">Multi-city/stopover</a>
        </div>
    </div>
    <div class="col-lg-2 col-md-6">
      <div>
      </div>
  </div>
  <div class="col-lg-3 col-md-6">
    <div>
    </div>
</div>
  </div>

        <div class="row no-gutters">
            <div class="col-lg-3 col-md-6">
              <div class="icon-box" style=" border-radius: 5px;border-style: outset; height: 200px;" data-bs-toggle="modal" data-bs-target="#myModal">
                <p>Leaving from</p>
                <p id="p1">{{ ita }}</p>
                <span id="p2">{{ cty }}</span>
            </div>
          </div>
          <div class="col-lg-3 col-md-6">
            <div class="icon-box" style=" border-radius: 5px; border-style: outset; height: 200px;" data-bs-toggle="modal" data-bs-target="#myModal1">
              <p>Going to</p>
              <p id="p1">{{ ita1 }}</p>
              <span id="p2">{{ cty1 }}</span>
          </div>
        </div>
        <div class="col-lg-3 col-md-6">
          <div class="icon-box" style=" border-radius: 5px; border-style: outset; height: 200px;" data-bs-toggle="modal" data-bs-target="#myModal2">
            <p>Departing on</p>
            <span id="p2">{{ dates.in }}</span>
            <hr>
            <!-- <HotelDatePicker /> -->
            <p>Returning on</p>
            <span id="p2">{{ dates.out }}</span>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class=" btn btn-info" type="button" id="c3" style="background-color:rgb(9, 67, 124); border-radius: 5px; height: 200px;" @click="getWeather()">
          <br><br><br>
          <img src="image/5.svg" height="50" width="100">
          <br><br><br>
      </div>
    </div>
        </div>
        <br>
        <div class="row no-gutters">
          <div class="col-lg-2 col-md-6">
              <div>
                <a  href="#" id="a1">Return <i class="fal fa-chevron-down"></i></a>
              </div>
          </div>
          <div class="col-lg-4 col-md-6">
            <div>
              <a  href="#" id="a1">Economy, 1 Audlt <i class="fal fa-chevron-down"></i></a>
            </div>
        </div>
        <div class="col-lg-3 col-md-6">
          <div>
          </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div>
        </div>
    </div>
      </div>
      <br>
        <div class="row no-gutters">
            <div class="col-lg-3 col-md-6">
                    <div class="card" style="width: 1100; background-color:rgb(9, 67, 124);">
                      <div class="card-body">
                        <h3 class="card-title" style="color:rgb(11, 146, 101)">"Tybee is replace with"</h3>
                        <br>
                        <a href="#" style="text-decoration: underline; color:rgb(11, 146, 101)">Find Perfectti</a><br>
                      </div>
                </div>
            </div>
            <div class="col-lg-3 col-md-6">
              <div class="card" style="width: 1100; background-color:rgb(9, 67, 124);">
                <div class="card-body">
                  <h3 class="card-title" style="color:rgb(11, 146, 101)">"Tybee is replace with"</h3>
                        <br>
                        <a href="#" style="text-decoration: underline; color:rgb(11, 146, 101)">Find Perfectti</a><br>
                </div>
          </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="card" style="width: 1100; background-color:rgb(9, 67, 124);">
          <div class="card-body">
            <h3 class="card-title" style="color:rgb(11, 146, 101)">"Tybee is replace with"</h3>
                        <br>
                        <a href="#" style="text-decoration: underline; color:rgb(11, 146, 101)">Find Perfectti</a><br>
          </div>
    </div>
</div>
<div class="col-lg-3 col-md-6">
  <div class="card" style="width: 1100; background-color:rgb(9, 67, 124);">
    <div class="card-body">
      <h3 class="card-title" style="color:rgb(11, 146, 101)">"Tybee is replace with"</h3>
                        <br>
                        <a href="#" style="text-decoration: underline; color:rgb(11, 146, 101)">Find Perfectti</a><br>
    </div>
</div>
</div>
        </div>
    </div>
    <div class="col-lg-4 col-md-6">
        <div class="row no-gutters">
            <div class="col-lg-12 col-md-6">
                <div class="icon-box">
                    <h6 class="descrip" style="padding: 0px 0px 0px 0px;">CATAGORIES</h6>
                    <p class="descrip">
                      <a href="">Alabama</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Arizona</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Beaches</a><br>
                      <a href="">California</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Florida</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Georgia</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Hawaii</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Hiking</a><br>
                      <a href="">Maine</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Maryland</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Massachusetts</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Museums</a><br>
                      <a href="">Oregon</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Parks</a><br>
                      <a href="">Place To Stay</a><br>
                      <a href="">Restaurants</a><br>
                      <a href="">South Carolina</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Tennessee</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Texas</a><a href=""><i class="fal fa-chevron-circle-down" style="float: right;"></i></a><br>
                      <a href="">Things to do</a><br><a href="">Tours</a><br><a href="">Uncategorized</a>
                    </p>
                </div>
            </div>
        </div>

    </div>
</div>
<div class="row no-gutters">
  <div class="col-lg-12 col-md-6">
    <div class="icon-box">
      <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
      <p class="fw-bold">Select Departing Flight</p> 
      <p>{{ cty }} to {{ cty1 }} {{ dates.out }}</p>
    </div>
  </div>
</div>
<div class="row no-gutters">
  <div class="col-lg-6 col-md-6">
    <div class="row no-gutters">
      <div class="col-lg-12 col-md-6">
        <!-- <div class="icon-box"> -->
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p>{{ dates.out }}, Forecast for {{ cty1 }}</p>
        <!-- </div> -->
      </div>
    </div>
    <div class="row no-gutters">
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
          <span class="card-text" style="color:black; font-size: 14px;">Morning</span>
          <h3 class="card-text" style="color:black;">70</h3>
          <span><i class='fas fa-smog' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
          <p style="color:black ;font-size:14px;">Some quick </p>
      </div>
    </div>
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Afternoon</span>
        <h3 class="card-text" style="color:black;">70</h3>
        <span><i class='fas fa-smog' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">Some quick </p>
    </div>
    </div>
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Evening</span>
        <h3 class="card-text" style="color:black;">70</h3>
        <span><i class='fas fa-smog' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">Some quick </p>
    </div>
    </div>
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Overnight</span>
        <h3 class="card-text" style="color:black;">70</h3>
        <span><i class='fas fa-smog' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">Some quick </p>
    </div>
    </div>
  </div>
</div>
  <div class="col-lg-6 col-md-6">
    <div class="row no-gutters">
      <div class="col-lg-12 col-md-6">
        <!-- <div class="icon-box"> -->
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p>{{ dates.out }}, Forecast for {{ cty1 }}</p>
        <!-- </div> -->
      </div>
    </div>
    <div class="row no-gutters">
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Morning</span>
        <h3 class="card-text" style="color:black;">{{ avg1 }}</h3>
        <span><i class='fas fa-smog' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">Some quick </p>
    </div>
    </div>
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Afternoon</span>
        <h3 class="card-text" style="color:black;">{{ avg2 }}</h3>
        <span><i class='fas fa-smog' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">Some quick </p>
    </div>
    </div>
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Evening</span>
        <h3 class="card-text" style="color:black;">{{ avg3 }}</h3>
        <span><i class='fas fa-smog' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">Some quick </p>
    </div>
    </div>
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Overnight</span>
        <h3 class="card-text" style="color:black;">{{ avg4 }}</h3>
        <span><i class='fas fa-smog' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">Some quick </p>
    </div>
    </div>
  </div>
</div>
</div>
<br>
<div class="row no-gutters">
  <div class="col-lg-6 col-md-6">
    <div class="row no-gutters">
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color:black ;font-size:12px;">Sort by:</p>
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color:black ;font-size:12px;">Recommended</p>
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color:black ;font-size:12px;">Departure time</p>
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color:black ;font-size:12px;">Arrival time </p>
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color:black ;font-size:12px;">Duration</p>
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color:black ;font-size:12px;">Fare</p>
      </div>
    </div>
    <div class="row no-gutters">
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color:black ;font-size:12px;">Sort by:</p>
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color:black ;font-size:12px;">Recommended</p>
      </div>
    </div>
    <div class="row no-gutters">
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p>View the lates</p>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p>View the lates</p>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p>View the lates</p>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p>View the lates</p>
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-6 col-md-6">
    <div class="row no-gutters">
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color:black ;font-size:12px;">Lowest Price</p>
      </div>
    </div>
    <div class="row no-gutters">
      <div class="col-lg-6 col-md-6">
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6" style="background-color:rgb(9, 67, 124)">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span class="fw-bold">2 latest updates </span>
          </div>
        </div>
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6">
            <div class="icon-box">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span class="fw-bold">2 latest updates </span> View the latest COVID-19 {{ jsondata.place }}
            </div>
          </div>
        </div>
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6">
            <div class="icon-box">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span class="fw-bold">2 latest updates </span> View the latest COVID-19 travel restrictions, quarentine requirenments and more
            </div>
          </div>
        </div>
      </div>
      <div class="col-lg-6 col-md-6">
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6" style="background-color:rgb(16, 37, 58)">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span class="fw-bold">2 latest updates </span>
          </div>
        </div>
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6">
            <div class="icon-box">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span class="fw-bold">2 latest updates </span> View the latest COVID-19 travel restrictions, quarentine requirenments and more
            </div>
          </div>
        </div>
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6">
            <div class="icon-box">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span class="fw-bold">2 latest updates </span> View the latest COVID-19 travel restrictions, quarentine requirenments and more
            </div>
          </div>
        </div>
      </div>
    </div>
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
import jData from "../data.json";
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
      cty1: "Coxs Bazar",
      ita1: "DAC",
      users1: [],
      gdate: "",
      dates: {
        in: "Jan 10 2022",
        out: "Jan 15 2022"
      },
      avg1: "19",
      avg2: "22",
      avg3: "30",
      avg4: "24",
      jsondata: jData

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
      //console.log(val.toString().slice(4,14));
      this.dates.in = val.toString().slice(4,16);
      this.gdate = val.toISOString().slice(0, 10);
      //console.log(moment(val).format('MM/DD/YYYY'));
    },
    checkOut(val) {
      console.log(val.toISOString().slice(0, 10));
      this.dates.out = val.toString().slice(4,16);
      //this.dates.out = val.toISOString().slice(0, 10);
    },

    getWeather(){
      axios
        .get(
           "http://api.weatherapi.com/v1/forecast.json?key=eb7d27b37d204bbbb2241423213112&q=" +
          this.cty1 +
          "&dt=" +
          this.dates.out   
        )
        .then(res => {
          //console.log(res.data.forecast.forecastday[0].hour[0].temp_c);
          // console.log(res.data.forecast);
          // var ho = res.data.forecast.forecastday[0].hour;
          // console.log(ho);
          //this.weather = res.data.forecast.forecastday[0];
          var sum1=0;
          var sum2=0;
          var sum3=0;
          var sum4=0;
          for(var i =0; i<24; i++) {
            if(i>=0 && i<6){
              sum1= sum1+res.data.forecast.forecastday[0].hour[i].temp_c;
            }   
            else if(i>=6 && i<12){
              sum2= sum2+res.data.forecast.forecastday[0].hour[i].temp_c;
            }
            else if(i>=12 && i<18){
              sum3= sum3+res.data.forecast.forecastday[0].hour[i].temp_c;
            }
            else if(i>=18 && i<24){
              sum4= sum4+res.data.forecast.forecastday[0].hour[i].temp_c;
            }
          }
          this.avg1= Math.round(sum1/6);
          this.avg2= Math.round(sum2/6);
          this.avg3= Math.round(sum3/6);
          this.avg4= Math.round(sum4/6);
          console.log(this.avg1);
          console.log(jsonData.place);
      
        })
        .catch(err => {
          console.log(err);
        });
    }
    
  }
}
</script>
<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    margin-top: 0px;
  }
  #nav {
    padding: 20px;
  }
  #nav a {
    font-weight: bold;
    color: #2c3e50;
  }
  #nav a.router-link-exact-active {
    color: #42b983;
  }
  
  a {
  text-decoration: none;
  color: #5cb874;
}

a:hover {
  color: #80c792;
  text-decoration: none;
}

h1, h2, h3, h4, h5, h6 {
  font-family: "Raleway", sans-serif;
}


.featured-services {
  padding: 20px 0;
}
.featured-services .icon-box {
  padding: 20px;
}
.featured-services .icon-box-bg {
  background-image: linear-gradient(0deg, #222222 0%, #2f2f2f 50%, #222222 100%);
}
.featured-services .icon {
  margin-bottom: 15px;
}
.featured-services .icon i {
  color: #5cb874;
  font-size: 42px;
}
.featured-services .title {
  font-weight: 700;
  margin-bottom: 15px;
  font-size: 18px;
}
.featured-services .title a {
  color: #ffffff;
  transition: 0.3s;
}
.featured-services .icon-box:hover .title a {
  color: #5cb874;
}
.featured-services .description {
  line-height: 24px;
  font-size: 14px;
}
.featured-services .description a {
  color: #ffffff;
}
.featured-services .icon-box:hover .description a {
  color: #5cb874;
}
.featured-services .descrip {
  line-height: 24px;
  font-size: 14px;
}
.featured-services .descrip a {
  color: #5cb874;
}
.featured-services .icon-box:hover .descrip a {
  color: #5cb874;
}
#p1 {
  font-size: 30px;
  font-weight: bold;
}
#p2 {
  font-size: 20px;
  font-weight: bold;
}
#c3 {
  background-repeat: no-repeat;
  height: 154px; width: 196px;
}
</style>
