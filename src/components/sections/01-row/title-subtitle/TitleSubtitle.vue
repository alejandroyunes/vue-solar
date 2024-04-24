<script lang="ts" setup>
import './title-subtitle.scss'

interface TitleSubtitleProps {
  title: string
  subtitle: string
}

const { title, subtitle } = defineProps<TitleSubtitleProps>()

</script>

<template>
  <section>
    <div class="title-subtitle-container">
      <div class="title">
        <p>{{ title }}</p>
      </div>
      <div class="subtitle">
        <p>{{ subtitle }}</p>
      </div>
    </div>
  </section>
</template>
