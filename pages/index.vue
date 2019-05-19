<template>
  <section class="container">
    <div>
      <logo />
      <h1 class="title">
        nuxt-seo
      </h1>
      <h2 class="subtitle">
        測試SEO Project
      </h2>
      <nuxt-link class="links" to="/about">About</nuxt-link>
      <nuxt-link class="links" to="/test">Test</nuxt-link>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  head: {
    title: 'Index Page',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'This is Eric Index page'
      },
      { property: 'og:title', content: 'Index Page' },
      { property: 'og:description', content: 'This is Eric Index page' },
      { property: 'og:site_name', content: 'Index Page' },
      { property: 'og:locale', content: 'zh_TW' },
      { property: 'og:image', content: '/index.png' }
    ],
    link: [{ rel: 'shortcut icon', href: '/index.png' }]
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  font-size: 42px;
  padding: 15px;
}
</style>
