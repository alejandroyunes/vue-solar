<script setup lang="ts">
import './blog-image.scss'
import { blogTitles } from './blogs-titles'
</script>


<template>
  <section class="blog-image-container">
    <router-link :to="`/blog/${blogInfo.id}`" v-for="blogInfo in blogTitles" :key="blogInfo.id">
      <div class="blog-item">

        <img class="image" :src="blogInfo.blogImage" alt="alt" width={300} height={200} />

        <div class="description">
          <h3 class="slogan">{{ blogInfo.category }}</h3>
          <p class="text">{{ blogInfo.title }}</p>
          <div class="bg">
            <p class="day">{{ blogInfo.day }}</p>
            <p>{{ blogInfo.month }}</p>
          </div>
        </div>
      </div>
    </router-link>
  </section>
</template>
