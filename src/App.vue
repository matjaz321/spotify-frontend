<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
    <playing-bar-footer/>
  </div>
</template>

<script>
import Footer from './views/Footer.vue';
export default {
  components: {
    'playing-bar-footer': Footer,
  }
}
</script>

<style lang="scss">
  @import 'styles/main.scss';
</style>
