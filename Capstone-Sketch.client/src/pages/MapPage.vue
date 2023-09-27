<template>
   <h1>
    User Location Page
   </h1>

  <!-- <head>
    <title>Simple Marker</title>
    <script src="https://polyfill.io/v3/polyfill.min.js?features=default"></script>
    <script src="https://maps.googleapis.com/maps/api/js?key=AIzaSyBifxFAXD3ecZoO52GpjV-STjO1LB1NnRg&callback=initMap&libraries=&v=weekly" defer></script>
  </head>
  <body>
    <div id="gmp-map"></div>
  </body> -->
</template>
    <script>
export default {
  setup() {
    return {

    }
  }
}

    //   "use strict";
    //   function initMap() {
    //     const myLatLng = {
    //       lat: 43.60671615600586,
    //       lng: -116.28668975830078
    //     };
    //     const map = new google.maps.Map(document.getElementById("gmp-map"), {
    //       zoom: 14,
    //       center: myLatLng,
    //       fullscreenControl: false,
    //       zoomControl: true,
    //       streetViewControl: false
    //     });
    //     new google.maps.Marker({
    //       position: myLatLng,
    //       map,
    //       title: "My location"
    //     });
    //   }
    </script>
          <style>
            /* Always set the map height explicitly to define the size of the div
             * element that contains the map. */
            #gmp-map {
              height: 100%;
            }
            /* Optional: Makes the sample page fill the window. */
            html,
            body {
              height: 100%;
              margin: 0;
              padding: 0;
            }
          </style>