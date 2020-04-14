<template>
<main class="">
  <div class="columns is-centered">

      <p class="orange has-text-white">
        Vi vet att det ibland kan vara svårt att bestämma vart man 
        ska gå för en AW eller en öl. <br>
        <br>
        Så därför har vi gjort det enkelt för dig att hitta,
        Använd vår Tapp-App och ta ett glas redan nu!
      </p>
      
      <a class="button" @click="$router.push('/Map')">Hitta nu!</a>
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
        max-width: 420px;
        line-height: 28px;
        font-size: 1.6rem;
        text-align: center;
        text-shadow: 1px 1px 2px rgb(109, 109, 109);
    }

    .button{
      width: 400px;
      padding: 20px;
      border-color: aliceblue;
      background-color: transparent;
      color: aliceblue;
      margin-top: 35px;
      font-size: 2rem;
      box-shadow: 7px 5px 5px rgba(172, 144, 85, 0.534);
    }

    .columns{
        width: 80%;
        display: flex;
        flex-direction: column;
        align-items: center;

    }
}
@media screen and (max-width: 500px) {

  main{
    height: 100vh;
    width: 100vw;
    display: flex;
    flex-direction: column;
    align-items: center;

    p{
        max-width: 400px;
        line-height: 28px;
        font-size: 1.4rem
    }

    .button{
      width: 95%;
      padding: 20px;
      border-color: aliceblue;
      background-color: transparent;
      color: aliceblue;
      margin-top: 185px;
      font-size: 2rem;
    }

    .columns{
        width: 80%;
        display: flex;
        flex-direction: column;
        align-items: center;

    }
}
}
    
</style>
