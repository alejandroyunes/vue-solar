<script lang="ts" setup>
import './social-hover.scss'
import DeezerSvg from './icons/DeezerSvg.vue'
import InstagramSvg from './icons/InstagramSvg.vue'
import SoundCloudSvg from './icons/SoundCloudSvg.vue'
import SportifySvg from './icons/SpotifySvg.vue'
import TwitterSvg from './icons/TwitterSvg.vue'
import YoutubeSvg from './icons/YoutubeSvg.vue'

</script>

<template>
  <section>
    <div class="social-hover-container">
      <div class="item-black">
        <DeezerSvg class="icon" />
      </div>

      <div class="item-light">
        <InstagramSvg class="icon" />
      </div>

      <div class="item-black">
        <SoundCloudSvg class="icon" />
      </div>

      <div class="item-light">
        <SportifySvg class="icon" />
      </div>

      <div class="item-black">
        <TwitterSvg class="icon" />
      </div>

      <div class="item-light">
        <YoutubeSvg class="icon" />
      </div>

    </div>

  </section>
</template>