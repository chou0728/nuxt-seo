<template>
  <section class="container">
    <div>
      <logo />
      <h1 class="title">
        This is About Page
      </h1>
      <p>
        About Page 的文字內容~~~~
      </p>
    </div>
  </section>
</template>

<script>
export default {
  head: {
    title: 'About Page',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'This is Eric About page'
      },
      { property: 'og:title', content: 'About Page' },
      { property: 'og:description', content: 'This is Eric About page' },
      { property: 'og:site_name', content: 'About Page' },
      { property: 'og:locale', content: 'zh_TW' },
      { property: 'og:image', content: '/about.png' }
    ],
    link: [{ rel: 'shortcut icon', href: '/about.png' }]
  }
}
</script>
