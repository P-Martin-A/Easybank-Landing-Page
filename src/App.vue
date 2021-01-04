<template>
  <div id="app">
    <Header />
    <Main />
    <Section />
    <Article />
    <Footer />
  </div>
</template>

<script>
  import Header from '@/layouts/Header'
  import Main from '@/layouts/Main'
  import Section from '@/layouts/Section'
  import Article from '@/layouts/Article'
  import Footer from '@/layouts/Footer'

  export default {
    name: 'App',
    components: {
      Header,
      Main,
      Section,
      Article,
      Footer
    }
  }
</script>