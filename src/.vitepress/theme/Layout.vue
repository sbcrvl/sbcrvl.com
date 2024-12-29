<script setup lang="ts">
import { useData } from 'vitepress'

// https://vitepress.dev/reference/runtime-api#usedata
const { site, frontmatter } = useData()
</script>

<template>
  <div v-if="frontmatter.home">
    <header>
      <a href="/">sbcrvl</a>
    </header>
    <Content />
  </div>
  <div v-else>
    <header>
      <a href="/">sbcrvl</a>
      <a href="/about">about</a>
    </header>
    <Content />
  </div>
</template>
