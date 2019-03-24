<template>
  <div class="now-playing__cover-art cover-art">
    <div
      class="cover-art__image cover-art--shadow art-logo"
      :class="`cover-art--${this.size}`"
    >
      <div>
        <div
          class="art-logo__default-logo"
          style="display: none;"
        >
          <DefaultArtLogo />
        </div>
        <div
          class="art-logo__art-cover"
          :style="artImageStyle()"></div>
      </div>
    </div>
  </div>
</template>

<script>
import DefaultArtLogo from '../assets/icons/DefaultArtLogo.svg'
export default {
  name: 'CoverArt',
  props: {
    size: {
      type: String,
      default: 'small'
    },
    artUrl: {
      type: String,
      required: true
    }
  },
  components: {
    DefaultArtLogo
  },
  methods: {

    artImageStyle () {
      return `background-image: url(${this.artUrl})`
    }
  }
}
</script>
