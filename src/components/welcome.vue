<template>
<main class="orange">
  <div class="columns is-centered">
      <p class="orange has-text-white">Vi vet att det ibland kan vara svårt att veta vart man ska gå för ett glas rött eller en öl, så vi har gjort det enkelt att hitta det närmsta stället för dig att ta reda på det. Använd vår krog lokaliserare och ta ett glas redan nu!</p>
    <a href="" class="button" @click="$router.push('/views/About')">Hitta nu!</a>
  </div>
  </main>
</template>

<script>
export default {
  name: 'welcome'
}
</script>

<style lang="scss">
main{
    height: 100vh;
    width: 100vw;
    display: flex;
    flex-direction: column;
    align-items: center;

    p{
        max-width: 350px;
        line-height: 28px;
        font-size: 1.4rem
    }

    .columns{
        width: 80%;
        display: flex;
        flex-direction: column;
        align-items: center;

    }
}
    
</style>
