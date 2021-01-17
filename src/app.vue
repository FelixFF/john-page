<template>
  <div id="app">
    <div class="container">
      <b-navbar id="nav">
        <template #brand>
          <b-navbar-item tag="router-link" :to="{ path: '/' }"> </b-navbar-item>
        </template>
        <template #start>
          <b-navbar-item tag="router-link" :to="{ path: '/' }">
            Home
          </b-navbar-item>
          <b-navbar-item tag="router-link" :to="{ path: '/about' }">
            About
          </b-navbar-item>
          <b-navbar-item tag="router-link" :to="{ path: '/contact' }">
            Contact
          </b-navbar-item>
          <b-navbar-item tag="router-link" :to="{ path: '/gallery' }">
            Gallery
          </b-navbar-item>
        </template>        
      </b-navbar>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">

html, body {
  height: 100%;
  margin: 0;
  padding: 0;
  overflow: auto !important;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  background-color: $true-blue;
  height: 100%;
}

.navbar-item {
  text-decoration: none;
  color: $oxford-blue;
}

#nav {
  a {
    font-weight: bold;
    color:$oxford-blue;

    &.router-link-exact-active {
      color: orange;
    }
  }
}
</style>
