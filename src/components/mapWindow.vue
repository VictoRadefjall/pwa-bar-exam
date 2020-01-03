<template>
<GmapMap
  :center="{lat:currentLocation.lat, lng:currentLocation.lng}"
  :zoom="17"
  :options="{disableDefaultUI:true}"
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

</template>

<script>
export default {
  name: 'mapwindow',
  mounted : function() {
    this.geolocation();
 },
  methods: {
    geolocation: function() {
      navigator.geolocation.getCurrentPosition((position) => {
        this.currentLocation = {
          lat: position.coords.latitude,
          lng: position.coords.longitude
        };
      });
    }
},
    data() {
    return {
      currentLocation : { lat : 0, lng : 0},
      searchAddressInput: ''
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
