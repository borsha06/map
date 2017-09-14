<template>
  <v-ons-page>
    <p style="text-align: center">
      Welcome home.
    </p>
    <div id="map"></div>
  </v-ons-page>
</template>

<script>

export default {
    data() {
        return {

        }
    },
    mounted: function() {
        this.initMap();
},
    methods: {
        initMap: function() {
            var map;
            map = new google.maps.Map(document.getElementById('map'), {
            center: {lat: 83.9207, lng: 35.9565},
            scrollwheel: false,
            zoom: 14
            })
        }
    }
}
</script>

<style>
#map 
{height:300px;width:500px;}
</style>

