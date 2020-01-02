<template>
<mapwindow class="half-screen"/>
</template>


<script>
import mapwindow from '@/components/mapWindow.vue';

export default {
  name: 'about',
  components: {
    mapwindow
  }
}



</script>

<style lang="scss">
.half-screen{
  height: 50vh;
  width: 100vw;

}
  
</style>
