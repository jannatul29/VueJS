<template>
  <div>
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
        placeholder="Going to"
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

</div>
</template>
<script>
import axios from "axios";

export default {
  data: function() {
    return {
      uname: "",
      unme: "",
      users: []
    }
  },

  methods: {
    getUser() {
        console.log(this.uname)
        axios.get("https://api.sharetrip.net/api/v1/flight/search/airport?name=" + this.uname)
        .then(res => {
                console.log("axios")
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
        this.props.uname = user.name
    },
    
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>