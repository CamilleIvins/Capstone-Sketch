<template>
  <section class="container">
    <section class="row justify-content-center">
      <!-- <div class="col-6 bg-primary">
qwerty
    </div> -->
    <div class="col-6 bg-danger">
<form action class="row">
  <!-- maxLength = Mick-proof this -->
  <input type="text" placeholder="address" class="col-10">

<i @click="locateButtonPressed()" class="col-1 mdi mdi-map-marker-outline"></i>

</form>
    </div>
    </section>
    

  </section>





</template>
<!-- video # 7 has error spin wheel rendering -->

<script>
import axios, { Axios } from 'axios';
import { AppState } from '../AppState';
import { computed, reactive, onMounted } from 'vue';
import { logger } from '../utils/Logger.js';
export default {
  setup(){
  return { 

    async locateButtonPressed(){

      if(navigator.geolocation){
      navigator.geolocation.getCurrentPosition(
        position => {
          // this.getAddressFrom(position.coords.latitude, position.coords.longitude)
          logger.log(position.coords.latitude);
          logger.log(position.coords.longitude);
        },
        error => {
          logger.log(error)
        },
      );
      } else {
        logger.log("Your browser does not support the geolocation API")
      }
    },
    async getAddressFrom(lat, long) {
    axios.get("https://maps.googleapis.com/maps/api/geocode/json?latlng=" + lat + "," + long + "&key=AIzaSyBifxFAXD3ecZoO52GpjV-STjO1LB1NnRg").then(response => {
      if(response.data.error_message){
        logger.log(response.data.error_message)
      } else {
        logger.log(response.data.results[0].formatted_address);
      }
    })
    }


   }
  }
};
</script>


<style lang="scss" scoped>
button{
  background-color: chocolate;
  color: whitesmoke;
}
</style>