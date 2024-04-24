<script lang="ts" setup>
import './title-subtitle.scss'

interface TitleSubtitleProps {
  title: string
  subtitle: string
  marginTop?: boolean
}

const { title, subtitle } = defineProps<TitleSubtitleProps>()

</script>

<template>
  <section class="title-subtitle-container">
    <div :class="{ 'extra-top-space': marginTop }">

      <div class="title">
        <p>{{ title }}</p>
      </div>

      <div class="subtitle">
        <p>{{ subtitle }}</p>
      </div>

    </div>
  </section>
</template>
