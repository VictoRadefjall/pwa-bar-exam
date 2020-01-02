<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/Sloggo.png">
    <welcome/>
  </div>
</template>

<script>
import welcome from '@/components/welcome.vue';

export default {
  name: 'home',
  components: {
    welcome
  }
}
</script>
<style lang="scss">
.home{
  background: linear-gradient(rgb(255, 123, 0), rgb(255, 196, 108));
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;

  img{
    margin: 25px;
    width: 300px;
    height: 250px;
  }
}
  
</style>
