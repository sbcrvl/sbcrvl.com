<script setup lang="ts">
import { useData } from 'vitepress'

// https://vitepress.dev/reference/runtime-api#usedata
const { site, frontmatter } = useData()
</script>

<template>
  <header>
    <div>
      <a href="/">sbcrvl</a>
      <span> / </span>
      <span>{{ frontmatter.breadcrumb }}</span>
    </div>
  </header>
  <Content />
</template>
