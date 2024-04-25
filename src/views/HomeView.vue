<script setup lang="ts">
import BillboardComponent from '@/components/billboard/billboard-fixed-top/BillboardFixed.vue'
import TitleSubtitle from '@/components/sections/01-row/title-subtitle/TitleSubtitle.vue'

import ImageTitle from '@/components/sections/02-row/image-title/ImageTitle.vue'
import CeoDescription from '@/components/sections/03-row/ceo-description/CeoDescription.vue'
import ImageDescription from '@/components/sections/02-row/image-description/ImageDescription.vue'
import PartnersComponent from '@/components/sections/01-row/partners/PartnersComponent.vue'
import GetInTouch from '@/components/sections/02-row/get-in-touch/GetInTouch.vue'
import IndentDescription from '@/components/sections/03-row/indent-description/IndentDescription.vue'
import ImageTitleOverlay from '@/components/sections/03-row/images-title-overlay/ImagesTitleOverlay.vue'
import UpcomingEvents from '@/components/sections/04-row/UpcomingEvents.vue'
</script>

<template>
  <BillboardComponent />

  <TitleSubtitle title="Great quality for your tracks" subtitle="OUR MUSIC STUDIO" />
  <IndentDescription />

  <TitleSubtitle title="Crafting Masterpieces" subtitle="Quality is our heartbeat" marginTop />
  <ImageTitleOverlay />

  <TitleSubtitle title="Upcoming Events" subtitle="Tour Dates 2024" />
  <UpcomingEvents />

  <ImageTitle />
  <CeoDescription />
  <ImageDescription />
  <PartnersComponent />
  <GetInTouch />
</template>
