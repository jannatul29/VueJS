<template>
    <div id="app">
      <nav class="container navbar navbar-expand-lg navbar-light bg-light" id="nav" style="background-color: teal">
          <a class="navbar-brand" href="#" style="text-shadow: 2px 2px;color: red; font-size: 25px;">FlightForYou.Com</a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
             <div class="navbar-nav ms-auto">
                    <li to="#" class="nav-item nav-link">Offers</li>
                    <li href="#" class="nav-item nav-link">Manage</li>
                    <li href="#" class="nav-link">Experience</li>
                    <li href="#" class="nav-link">Marco Polo Club</li>
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
            <a  href="#" id="a1" style="color: rgb(9, 67, 124)">Rendom flights</a>
          </div>
      </div>
      <div class="col-lg-4 col-md-6">
        <div>
          <a  href="#" id="a1" style="color: rgb(9, 67, 124)">Multi-city/stopover</a>
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
          <div class="icon-box btn btn-info" type="button" style="background-color:rgb(9, 67, 124); border-radius: 5px; border-style: outset; height: 200px;" @click="getWeather()" href="#top">
            <a href="#top"><br><i class="fa fa-plane" style=" color: white; text-align: center"></i>
            <br><br><br></a>
            <a href="#top" style=" color: white; text-align: center"><h5>Search flights</h5>
            <br><br></a>
        </div>
      </div>

      
        </div>
        <br>
        <div class="row no-gutters">
          <div class="col-lg-2 col-md-6">
              <div>
                <a  href="#" id="a1" style="color: rgb(9, 67, 124)">Return <i class="fal fa-chevron-down"></i></a>
              </div>
          </div>
          <div class="col-lg-4 col-md-6">
            <div>
              <a  href="#" id="a1" style="color: rgb(9, 67, 124)">Economy, 1 Audlt <i class="fal fa-chevron-down"></i></a>
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
                        <h3 class="card-title" style="color: white; text-align: center"><i class="fas fa-bars"></i></h3>
                        <p style=" color: white; text-align: center">Manage booking</p>
                      </div>
                </div>
            </div>
            <div class="col-lg-3 col-md-6">
              <div class="card" style="width: 1100; background-color:rgb(9, 67, 124);">
                <div class="card-body">
                  <h3 class="card-title" style="color: white; text-align: center"><i class="fas fa-bars"></i></h3>
                        <p style=" color: white; text-align: center">Check in</p>
                </div>
          </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="card" style="width: 1100; background-color:rgb(9, 67, 124);">
          <div class="card-body">
            <h3 class="card-title" style="color: white; text-align: center"><i class="fas fa-exchange-alt"></i></h3>
                        <p style=" color: white; text-align: center">Rebook and refund</p>
          </div>
    </div>
</div>
<div class="col-lg-3 col-md-6">
  <div class="card" style="width: 1100; background-color:rgb(9, 67, 124);">
    <div class="card-body">
      <h3 class="card-title" style="color: white; text-align: center"><i class="fas fa-shield-virus"></i></h3>
                        <p style=" color: white; text-align: center">COVID-19 updates</p>
    </div>
</div>
</div>
        </div>
    </div>
    <div class="col-lg-4 col-md-6" style= "background: url(./assets/logo.png); background-repeat: no-repeat;background-size: cover;">
        <div class="row no-gutters">
            <div class="col-lg-12 col-md-6">
                <div class="icon-box">
                  <br>
                  <img src="./assets/images.jpg" style="object-fit: inherit;" height="450" width= "400">
                </div>
            </div>
        </div>
    </div>
</div>
<div class="row no-gutters" id="top">
  <div class="col-lg-12 col-md-6">
    <div class="icon-box">
      <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
      <p class="fw-bold" style="color: rgb(9, 67, 124)">Select Departing Flight</p> 
      <p><span class="fw-bold">{{ cty }}</span> to <span class="fw-bold">{{ cty1 }}</span> {{ dates.out }}</p>
    </div>
  </div>
</div>
<div class="row no-gutters">
  <div class="col-lg-6 col-md-6">
    <div class="row no-gutters">
      <div class="col-lg-12 col-md-6">
        <!-- <div class="icon-box"> -->
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p>{{ dates.out }}, <span class="fw-bold">Forecast for {{ cty1 }}</span></p>
        <!-- </div> -->
      </div>
    </div>
    <div class="row no-gutters">
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
          <span class="card-text" style="color:black; font-size: 14px;">Morning</span>
          <h3 class="card-text" style="color:black;">70&deg;</h3>
          <span><i class='fas fa-cloud-sun' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
          <p style="color:black ;font-size:14px;">Some quick </p>
      </div>
    </div>
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Afternoon</span>
        <h3 class="card-text" style="color:black;">70&deg;</h3>
        <span><i class='fas fa-cloud-hail-mixed' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">Some quick </p>
    </div>
    </div>
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Evening</span>
        <h3 class="card-text" style="color:black;">70&deg;</h3>
        <span><i class='fas fa-cloud-moon-rain' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">Some quick </p>
    </div>
    </div>
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Overnight</span>
        <h3 class="card-text" style="color:black;">70&deg;</h3>
        <span><i class='fas fa-cloud-moon' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
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
          <p>{{ dates.out }}, <span class="fw-bold">Forecast for {{ cty1 }}</span></p>
        <!-- </div> -->
      </div>
    </div>
    <div class="row no-gutters">
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Morning</span>
        <h3 class="card-text" style="color:black;">{{ avg1 }}&deg;</h3>
        <span><i class='fas fa-cloud-sun' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">{{ ar1 }}% </p>
    </div>
    </div>
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Afternoon</span>
        <h3 class="card-text" style="color:black;">{{ avg2 }}&deg;</h3>
        <span><i class='fas fa-cloud-hail-mixed' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">{{ ar2 }}%</p>
    </div>
    </div>
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Evening</span>
        <h3 class="card-text" style="color:black;">{{ avg3 }}&deg;</h3>
        <span><i class='fas fa-cloud-moon-rain' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">{{ ar3 }}%</p>
    </div>
    </div>
    <div class="col-lg-3 col-md-6">
      <div class="card" style="text-align: center">
        <span class="card-text" style="color:black; font-size: 14px;">Overnight</span>
        <h3 class="card-text" style="color:black;">{{ avg4 }}&deg;</h3>
        <span><i class='fas fa-cloud-moon' style='font-size:24px; color:rgb(106, 106, 211);'></i></span>
        <p style="color:black ;font-size:14px;">{{ ar4 }}%</p>
    </div>
    </div>
  </div>
</div>
</div>
<br>
<div class="row no-gutters">
  <div class="col-lg-6 col-md-6">
    <div class="row no-gutters">
      <div class="col-lg-3 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color:black ;font-size:12px;">Sort by: <span style="color: rgb(9, 67, 124)">Recommended</span></p>
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color: rgb(9, 67, 124) ;font-size:12px;">Departure time</p>
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color: rgb(9, 67, 124) ;font-size:12px;">Arrival time </p>
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color: rgb(9, 67, 124) ;font-size:12px;">Duration</p>
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color: rgb(9, 67, 124) ;font-size:12px;">Fare</p>
      </div>
      <div class="col-lg-1 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> --> 
      </div>
    </div>
    <div class="row no-gutters">
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color:black ;font-size:12px;">5 flights found</p>
      </div>
      <div class="col-lg-2 col-md-6">
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <p style="color: rgb(9, 67, 124) ;font-size:12px;">Filter <i class="fal fa-chevron-down"></i></p>
      </div>
    </div>
    <div class="row no-gutters" style="text-align:center">
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <br>
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <span style="color: rgb(9, 67, 124) ;font-size:20px;">{{ jsondata.st.start }}</span><br>
          <span class="fw-bold" style="font-size:12px;">{{ cty }}</span>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <br>
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <span style="color: black ;font-size:12px;">{{ jsondata.st.duration }}</span><br>
          <span class="fw-bold" style="font-size:12px; color: rgb(9, 67, 124) ;">LAX</span>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <br>
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <span style="color: rgb(9, 67, 124) ;font-size:20px;">{{ jsondata.st.end }}</span><br>
          <span class="fw-bold" style="font-size:12px;">{{ cty1 }}</span>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <br>
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <span style="color: black ;font-size:13px;">CX880 <i class="fal fa-chevron-right"></i> CX7906</span><br>
          <span style="font-size:12px; color: rgb(9, 67, 124)">View details <i class="fal fa-chevron-down"></i></span>
        </div>
      </div>
    </div>
    <div class="row no-gutters" style="text-align:center">
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <br>
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <span style="color: rgb(9, 67, 124) ;font-size:20px;">{{ jsondata.nd.start }}</span><br>
          <span class="fw-bold" style="font-size:12px;">{{ cty }}</span>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <br>
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <span style="color: black ;font-size:12px;">{{ jsondata.nd.duration }}</span><br>
          <span class="fw-bold" style="font-size:12px; color: rgb(9, 67, 124) ;">LAX</span>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <br>
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <span style="color: rgb(9, 67, 124) ;font-size:20px;">{{ jsondata.nd.end }}</span><br>
          <span class="fw-bold" style="font-size:12px;">{{ cty1 }}</span>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <br>
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <span style="color: black ;font-size:13px;">CX880 <i class="fal fa-chevron-right"></i> AA2002</span><br>
          <span style="font-size:12px; color: rgb(9, 67, 124)">View details <i class="fal fa-chevron-down"></i></span>
        </div>
      </div>
    </div>
    <div class="row no-gutters" style="text-align:center">
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <br>
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <span style="color: rgb(9, 67, 124) ;font-size:20px;">{{ jsondata.rd.start }}</span><br>
          <span class="fw-bold" style="font-size:12px;">{{ cty }}</span>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <br>
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <span style="color: black ;font-size:12px;">{{ jsondata.rd.duration }}</span><br>
          <span class="fw-bold" style="font-size:12px; color: rgb(9, 67, 124) ;">LAX</span>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <br>
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <span style="color: rgb(9, 67, 124) ;font-size:20px;">{{ jsondata.rd.end }}</span><br>
          <span class="fw-bold" style="font-size:12px;">{{ cty1 }}</span>
        </div>
      </div>
      <div class="col-lg-3 col-md-6">
        <div class="icon-box">
          <br>
          <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
          <span style="color: black ;font-size:13px;">CX880 <i class="fal fa-chevron-right"></i> AA2475</span><br>
          <span style="font-size:12px; color: rgb(9, 67, 124)">View details <i class="fal fa-chevron-down"></i></span>
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
      <div class="col-lg-6 col-md-6" style="text-align: center">
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6" style="background-color:rgb(9, 67, 124)">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span class="fw-bold" style="color: white">Economy</span>
          </div>
        </div>
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6" style="border-bottom-style: solid; border-bottom-color: rgb(9, 67, 124);">
            <div class="icon-box" style="color:rgb(9, 67, 124)">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span style="font-size:12px;">From</span><br>
              <span>{{ jsondata.economy.price1 }}</span><br>
              <span style="font-size:12px;">View fare <i class="fal fa-chevron-down"></i></span>
            </div>
          </div>
        </div>
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6" style="border-bottom-style: solid; border-bottom-color: rgb(9, 67, 124);">
            <div class="icon-box" style="color:rgb(9, 67, 124)">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span style="font-size:12px;">From</span><br>
              <span>{{ jsondata.economy.price2 }}</span><br>
              <span style="font-size:12px;">View fare <i class="fal fa-chevron-down"></i></span>
            </div>
          </div>
        </div>
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6" style="border-bottom-style: solid; border-bottom-color: rgb(9, 67, 124);">
            <div class="icon-box" style="color:rgb(9, 67, 124)">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span style="font-size:12px;">From</span><br>
              <span>{{ jsondata.economy.price3 }}</span><br>
              <span style="font-size:12px;">View fare <i class="fal fa-chevron-down"></i></span>
            </div>
          </div>
        </div>
      </div>
      <div class="col-lg-6 col-md-6" style="text-align: center">
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6" style="background-color:steelblue">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span class="fw-bold" style="color: white">Premium Economy</span>
          </div>
        </div>
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6" style="border-bottom-style: solid; border-bottom-color: rgb(9, 67, 124);">
            <div class="icon-box" style="color:rgb(9, 67, 124)">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span style="font-size:12px;">From</span><br>
              <span>{{ jsondata.premium.price1 }}</span><br>
              <span style="font-size:12px;">View fare <i class="fal fa-chevron-down"></i></span>
            </div>
          </div>
        </div>
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6" style="border-bottom-style: solid; border-bottom-color: rgb(9, 67, 124);">
            <div class="icon-box" style="color:rgb(9, 67, 124)">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span style="font-size:12px;">From</span><br>
              <span>{{ jsondata.premium.price1 }}</span><br>
              <span style="font-size:12px;">View fare <i class="fal fa-chevron-down"></i></span>
            </div>
          </div>
        </div>
        <div class="row no-gutters">
          <div class="col-lg-12 col-md-6" style="border-bottom-style: solid; border-bottom-color: rgb(9, 67, 124);">
            <div class="icon-box" style="color:rgb(9, 67, 124)">
              <!-- <h2 class="title1" style="color: white;">The Best Sedona Hiking Trails</h2> -->
              <span style="font-size:12px;">From</span><br>
              <span>{{ jsondata.premium.price1 }}</span><br>
              <span style="font-size:12px;">View fare <i class="fal fa-chevron-down"></i></span>
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
      cty: "place",
      ita: "Select",
      users: [],
      uname1: "",
      cty1: "place",
      ita1: "Select",
      users1: [],
      gdate: "",
      dates: {
        in: "Select date",
        out: "Select date"
      },
      avg1: "19",
      avg2: "22",
      avg3: "30",
      avg4: "24",
      ar1: "0",
      ar2: "0",
      ar3: "0",
      ar4: "0",
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
          var r1 = 0;
          var r2 = 0;
          var r3 = 0;
          var r4 = 0;
          for(var i =0; i<24; i++) {
            if(i>=0 && i<6){
              sum1= sum1+res.data.forecast.forecastday[0].hour[i].temp_c;
              r1= r1+res.data.forecast.forecastday[0].hour[i].chance_of_rain;
            }   
            else if(i>=6 && i<12){
              sum2= sum2+res.data.forecast.forecastday[0].hour[i].temp_c;
              r1= r1+res.data.forecast.forecastday[0].hour[i].chance_of_rain;
            }
            else if(i>=12 && i<18){
              sum3= sum3+res.data.forecast.forecastday[0].hour[i].temp_c;
             r1= r1+res.data.forecast.forecastday[0].hour[i].chance_of_rain;
            }
            else if(i>=18 && i<24){
              sum4= sum4+res.data.forecast.forecastday[0].hour[i].temp_c;
              r1= r1+res.data.forecast.forecastday[0].hour[i].chance_of_rain;
            }
          }
          this.avg1= Math.round(sum1/6);
          this.avg2= Math.round(sum2/6);
          this.avg3= Math.round(sum3/6);
          this.avg4= Math.round(sum4/6);

          this.ar1= Math.round(r1/6);
          this.ar2= Math.round(r2/6);
          this.ar3= Math.round(r3/6);
          this.ar4= Math.round(r4/6);
          console.log(this.avg1);
          //console.log(jsonData.place);
          console.log(res.data.forecast.forecastday[0].hour[0].chance_of_rain);
      
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

</style>
