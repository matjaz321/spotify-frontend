<template>
  <div class="main-boxes">
    <div class="main-boxes__header">
      <h1>Make yourself comfortable</h1>
    </div>
    <div class="main-boxes__content">
      <div class="grid-layout">
        <div class="grid-item">
          <Box
            :art-url="'https://pl.scdn.co/images/pl/default/a1f8040e8f297fff2d7be6efe8d1a0f250a30490'"
            :title="'Happy Dance'"
          />
        </div>
        <div class="grid-item">
          <Box
            :art-url="'https://pl.scdn.co/images/pl/default/fb8f51f74d738a62fbba6d715abe1ee2bd4ec4f8'"
            :title="'Feelgood Indie'"
          />
        </div>
        <div class="grid-item">
          <Box
            :art-url="'https://pl.scdn.co/images/pl/default/d376cd0266b552035f73c458face3ddf88a7761e'"
            :title="'Jazz Vibes'"
          />
        </div>
        <div class="grid-item">
          <Box
            :art-url="'https://pl.scdn.co/images/pl/default/b0d7bf46749225061b9ce14428bd28e485ddd4fb'"
            :title="'Spring Feelings'"
          />
        </div>
        <div class="grid-item">
          <Box
            :art-url="'https://pl.scdn.co/images/pl/default/d519e1e7ba7ddbdb48fc84944753ed990392a2b5'"
            :title="'Chillout Lounge'"
          />
        </div>
        <div class="grid-item">
          <Box
            :art-url="'https://pl.scdn.co/images/pl/default/a85183fe886b2aa2d83e5de1b199f0d04bf22dc0'"
            :title="'Feelgood Pop'"
          />
        </div>
        <div class="grid-item">
          <Box
            :art-url="'https://pl.scdn.co/images/pl/default/74b6f34ee1c98f8e2c5daa8f553def6b1eab4b31'"
            :title="'Spring Chillout'"
          />
        </div>
        <div class="grid-item">
          <Box
            :art-url="'https://pl.scdn.co/images/pl/default/7852401044ad35b77d081b858dad431a061d7f8f'"
            :title="'Pop Brandneu'"
          />
        </div>
        <div class="grid-item">
          <Box
            :art-url="'https://pl.scdn.co/images/pl/default/3bf56d42dd2c4f9348b934401e1f820a369a4580'"
            :title="'At home'"
          />
        </div>
        <div class="grid-item">
          <Box
            :art-url="'https://pl.scdn.co/images/pl/default/4c272c8ebba07c309a780ddf51c4f2ee84f28346'"
            :title="'Clear edge'"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Box from '../components/Box'
export default {
  name: 'MainBoxes',
  components: {
    Box
  }
}
</script>
