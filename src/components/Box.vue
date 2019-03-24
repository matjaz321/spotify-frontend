<template>
  <div class="box">
    <div class="box__info">
      <div class="box__art">
        <CoverArt
          :art-url="artUrl"
          size="max"
        />
      </div>
      <div class="box__info-wrapper">
        <a href="#">
          {{ title }}
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import CoverArt from './CoverArt'
export default {
  name: 'Box',
  components: {
    CoverArt
  },
  props: {
    artUrl: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    }
  }
}
</script>
