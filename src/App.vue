<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <div class="main-content">
      <router-view />
      <main-sidebar />
      <main-view />
    </div>
    <playing-bar-footer />
  </div>
</template>

<script>
import Footer from './views/Footer'
import Sidebar from './views/Sidebar'
import MainView from './views/MainView'

export default {
  components: {
    'playing-bar-footer': Footer,
    'main-sidebar': Sidebar,
    'main-view': MainView
  }
}
</script>

<style lang="scss">
  @import 'styles/main.scss';
</style>
