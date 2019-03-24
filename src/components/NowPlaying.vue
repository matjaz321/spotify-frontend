<template>
  <div class="now-playing">
    <span class="now-playing__widget-overlay">
      <a
        aria-label="Now playing: Say My Name (feat. Bebe Rexha & J Balvin) - Lucas & Steve Remix by David Guetta, Bebe Rexha, J Balvin, Lucas & Steve"
        href="/playlist/123"
      >
        <div class="now-playing__cover-art cover-art">
          <div class="cover-art__image cover-art--shadow art-logo">
            <div>
              <div
                class="art-logo__default-logo"
                style="display: none;"
              >
                <DefaultArtLogo />
              </div>
              <div
                class="art-logo__art-cover"
                style="background-image: url('https://i.scdn.co/image/bded386db47dd4a502fd3c354b98bd068e01c4d8');">
              </div>
            </div>
          </div>
        </div>
      </a>
    </span>
    <div class="now-playing__track-info track-info">
      <div class="track-info__name">
        <a href="/album/123">
          Bones (feat. OneRepublic)
        </a>
      </div>
      <div class="track-info__artists">
        <span href="/artist/4sTQVOfp9vEMCemLw50sbu">
          Galantis
        </span>
        <span href="/artist/4sTQVOfp9vEMCemLw50sbu">
          OneRepublic
        </span>
      </div>
    </div>
    <save-to-playlist />
  </div>
</template>

<script>
import SaveToPlaylist from './SaveToPlaylist'

import DefaultArtLogo from '../assets/icons/DefaultArtLogo.svg'

export default {
  name: 'NowPlaying',
  components: {
    SaveToPlaylist,
    DefaultArtLogo
  },
  data () {
    return {

    }
  }
}

</script>
