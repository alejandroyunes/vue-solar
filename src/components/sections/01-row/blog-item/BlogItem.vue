<script setup lang="ts">
import './blog-item.scss'
import { blogTitles } from '../../03-row/blog-image-description/blogs-titles'
import { useRoute } from 'vue-router'

const route = useRoute()
const id = Number(route.params.id)

const filteredBlog = blogTitles.filter(item => item.id === id)

</script>

<template>
  <section class="blog-item-container" v-for="item in filteredBlog" :key="item.id">
    <h1 class="title">{{ item.title }}</h1>
    <img class="image" :src="item.blogImage" alt="" width={600} height={400} />

    <p>{{ item.blogSection1 }}</p>
    <br />
    <p>{{ item.blogSection2 }}</p>
    <br />
    <p>{{ item.blogSection3 }}</p>
    <br />
    <p>{{ item.blogSection4 }}</p>
    <br />
  </section>

</template>
