<script setup lang="ts">
import BillboardComponent from '@/components/billboard/billboard-fixed-top/BillboardFixed.vue'
import TitleSubtitle from '@/components/sections/01-row/title-subtitle/TitleSubtitle.vue'
import ImageDescription from '@/components/sections/03-row/image-description/ImageDescription.vue'
import ImageTitle from '@/components/sections/02-row/image-title/ImageTitle.vue'
import CardDescription from '@/components/sections/04-row/card-description/CardDescription.vue'
import GetInTouch from '@/components/sections/02-row/get-in-touch/GetInTouch.vue'
</script>

<template>
  <BillboardComponent />
  <TitleSubtitle title="Elevate your world Sun-Powered Solutions" subtitle="" marginTop />

  <CardDescription />


  <ImageTitle />

  <TitleSubtitle title="Explore Energy Savings, Efficiency Devices, and Expert Consultations" subtitle="Our process"
    marginTop />
  <ImageDescription />

  <GetInTouch />
</template>
