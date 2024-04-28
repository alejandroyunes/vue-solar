<script setup lang="ts">
import BillboardComponent from '@/components/billboard/billboard-fixed-top/BillboardFixed.vue'
import TitleSubtitle from '@/components/sections/01-row/title-subtitle/TitleSubtitle.vue'
import IndentDescription from '@/components/sections/03-row/indent-description/IndentDescription.vue'
import ImageTitleOverlay from '@/components/sections/03-row/images-title-overlay/ImagesTitleOverlay.vue'
import UpcomingEvents from '@/components/sections/04-row/UpcomingEvents.vue'
import ImageGrid from '@/components/sections/03-row/images-grid/ImageGrid.vue'
import SocialHover from '@/components/sections/06-row/social-hover/SocialHover.vue'
</script>

<template>
  <BillboardComponent />

  <TitleSubtitle title="Elevate your world Sun-Powered Solutions" subtitle="" />
  <IndentDescription />

  <TitleSubtitle title="Crafting Masterpieces" subtitle="Quality is our heartbeat" marginTop />
  <ImageTitleOverlay />

  <TitleSubtitle title="Upcoming Events" subtitle="Tour Dates 2024" />
  <UpcomingEvents />

  <ImageGrid />

  <SocialHover />

</template>
