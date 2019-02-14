<template>
  <div class="now-playing">
    <span class="now-playing__widget-overlay">
      <a aria-label="Now playing: Say My Name (feat. Bebe Rexha & J Balvin) - Lucas & Steve Remix by David Guetta, Bebe Rexha, J Balvin, Lucas & Steve"
        href="/playlist/123">
        <div class="now-playing__cover-art cover-art">
          <div class="cover-art__image cover-art--shadow art-logo">
            <div>
              <div class="art-logo__default-logo" style="display: none;">
                <svg width="80" height="81" viewBox="0 0 80 81" xmlns="http://www.w3.org/2000/svg">
                  <title>Playlist Icon</title>
                  <path d="M25.6 11.565v45.38c-2.643-3.27-6.68-5.37-11.2-5.37-7.94 0-14.4 6.46-14.4 14.4s6.46 14.4 14.4 14.4 14.4-6.46 14.4-14.4v-51.82l48-10.205V47.2c-2.642-3.27-6.678-5.37-11.2-5.37-7.94 0-14.4 6.46-14.4 14.4s6.46 14.4 14.4 14.4S80 64.17 80 56.23V0L25.6 11.565zm-11.2 65.61c-6.176 0-11.2-5.025-11.2-11.2 0-6.177 5.024-11.2 11.2-11.2 6.176 0 11.2 5.023 11.2 11.2 0 6.174-5.026 11.2-11.2 11.2zm51.2-9.745c-6.176 0-11.2-5.024-11.2-11.2 0-6.174 5.024-11.2 11.2-11.2 6.176 0 11.2 5.026 11.2 11.2 0 6.178-5.026 11.2-11.2 11.2z"
                    fill="currentColor" fill-rule="evenodd"></path>
                </svg>
              </div>
              <div class="art-logo__art-cover" style="background-image: url('https://i.scdn.co/image/bded386db47dd4a502fd3c354b98bd068e01c4d8');">
              </div>
            </div>
          </div>
        </div>
      </a>
    </span>
    <div class="now-playing__track-info track-info">
      <div class="track-info__name">
        <a href="/album/123">Bones (feat. OneRepublic)</a>
      </div>
      <div class="track-info__artists">
        <span href="/artist/4sTQVOfp9vEMCemLw50sbu">Galantis</span>
        <span href="/artist/4sTQVOfp9vEMCemLw50sbu">OneRepublic</span>
      </div>
    </div>
    <save-to-playlist/>
  </div>
</template>

<script>
  import SaveToPlaylist from './SaveToPlaylist';

  export default {
    name: 'NowPlaying',
    components: {
      SaveToPlaylist,
    },
    data() {
      return {

      };
    },
  }

</script>
