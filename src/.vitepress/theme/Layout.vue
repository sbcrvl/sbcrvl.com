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
  <main>
    <Content />
  </main>
  <hr>
  <footer>
    <nav>
      <div>
        <a href="/about">About</a>
        <a href="/work">Work</a>
        <a href="/blog">Blog</a>
        <a href="/contact">Contact</a>
      </div>
      <div>
        <a href="/photos">Photos</a>
        <a href="/notes">Notes</a>
        <a href="/books">Books</a>
        <a href="/things">Things</a>
      </div>
    </nav>

    <section>
      <img src="" alt="">

      <div>
        <a href="/colophon">Colophon</a>
        <span> · </span>
        <a href="mailto:sbcrvl@gmail.com">Mail</a>
      </div>
    </section>
  </footer>
</template>
