<template>
<div>

<mapwindow class="half-screen"/>
<places/>

</div>
</template>


<script>
import mapwindow from '@/components/mapWindow.vue';
import places from '@/components/placebar.vue';

export default {
  name: 'map',
  components: {
    mapwindow,
    places
  }
}



</script>

<style lang="scss">
.half-screen{
  height: 50vh;
  width: 100vw;

}
  
</style>
