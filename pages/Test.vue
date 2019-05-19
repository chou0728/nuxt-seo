<template>
  <section class="container">
    <div>
      <logo />
      <h1 class="title">
        This is Test Page
      </h1>
      <p>
        Test Page 的文字內容~~~~
      </p>
    </div>
  </section>
</template>

<script>
export default {
  head: {
    title: 'Test Page',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'This is Eric test page'
      },
      { property: 'og:title', content: 'Test Page' },
      { property: 'og:description', content: 'This is Eric test page' },
      { property: 'og:site_name', content: 'Test Page' },
      { property: 'og:locale', content: 'zh_TW' },
      { property: 'og:image', content: '/test.png' }
    ],
    link: [{ rel: 'shortcut icon', href: '/test.png' }]
  }
}
</script>
