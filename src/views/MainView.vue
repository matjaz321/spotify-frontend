<template>
  <div class="inside-view">
    <div class="inside-view__container">
      <div class="inside-content">
        <MainNavigation />
        <MainBoxes />
      </div>
    </div>
  </div>
</template>

<script>
import MainNavigation from '../components/MainNavigation'
import MainBoxes from '../components/MainBoxes'
export default {
  name: 'MainView',
  components: {
    MainNavigation,
    MainBoxes
  }
}
</script>
