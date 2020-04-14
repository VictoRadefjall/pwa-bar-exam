<template>
  <div>
      <h2>Sök på vilken typ av lokal du vill hitta (ex. bar, pub, longe)</h2>
      <label>
        <gmap-autocomplete
          @place_changed="setPlace">
        </gmap-autocomplete>
        <button @click="addMarker">Add</button>
      </label>
      <br/>
  

<GmapMap
  :center="{lat:currentLocation.lat, lng:currentLocation.lng}"
  :zoom="14"
  :options="{disableDefaultUI:false}"
  map-type-id="terrain"
  style="width: 100vw; height: 50vh;"
>
  <GmapMarker
    :key="index"
    v-for="(m, index) in markers"
    :position="m.position"
    :clickable="true"
    :draggable="true"
    @click="center=m.position"
  />
</GmapMap>
</div>
</template>



<script>
import { gmapApi } from 'vue2-google-maps';

export default {
  name: 'mapwindow',

 computed: {
     google: gmapApi,
 },
 mounted: function() {
    this.geolocation();
 },
methods: {
    setPlace(place) {
      this.geolocation = place;
    },
    addMarker() {
      if (this.currentPlace) {
        const marker = {
          lat: this.currentPlace.geometry.location.lat(),
          lng: this.currentPlace.geometry.location.lng()
        };
        this.markers.push({ position: marker });
        this.places.push(this.currentPlace);
        this.center = marker;
        this.currentPlace = null;
      }
    },
    geolocation: function() {
      navigator.geolocation.getCurrentPosition((position) => {
        this.currentLocation = {
          lat: position.coords.latitude,
          lng: position.coords.longitude
        };
      });
    },
    // searchLocation: function() {
    //   var geocoder = new google.maps.Geocoder();
    //   geocoder.geocode({'address': this.searchAddressInput}, (results, status) => {
    //     if (status === 'OK') {
    //       this.currentLocation.lat = results[0].geometry.location.lat();
    //       this.currentLocation.lng = results[0].geometry.location.lng();
    //     }
    //   });
    // }
},
data() {
    return {
      markers: [10],
      places: [10],      
      currentLocation : { lat : 0, lng : 0},
      searchAddressInput: 'Pub',
      currentPlace: null,
      center: { lat: 45.508, lng: -73.587 }
    }
  } 
}
</script>

<style lang="scss">
main{
    height: 100vh;
    width: 100vw;
    display: flex;
    flex-direction: column;
    align-items: center;

    .columns{
        width: 80%;
        display: flex;
        flex-direction: column;
        align-items: center;

        .column{
            margin: 15px;
            width: 100%;
        }

    }
}
    
</style>
