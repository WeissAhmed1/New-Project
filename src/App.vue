<template>
  <div id="app">
    <div>
  <div>
  <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand href="#"><E-Library>E-Library</E-Library></b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

   
  <div>
  <div class="mt-3">
  <b-button-group>
  <b-button variant="success">
  <router-link to="/">Home</router-link>
  </b-button>
  <b-button variant="warning">
  <router-link to="/about">About</router-link>

  </b-button>
  </b-button-group>
  </div>
</div>
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
        </b-nav-form>
        <b-button variant="success">profile</b-button>

      </b-navbar-nav>
  </b-navbar>
</div>
</div>

    <router-view/>





  </div>  
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.router-link-active {
  margin-right: 20px;
}

#nav {

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>

