<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Hem</router-link> |
      <router-link to="/Map">Sök</router-link> |
      <router-link to="/CloseFind">Hitta lokal</router-link>
    </div>
    <router-view/>
  </div>
</template>


<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #c48322;
    }
  }
}
</style>
