<template>
  <b-container fluid id="main-container">
    <Header />
    <nuxt />
    <Footer />
  </b-container>
</template>

<script>
  import Header from '~/components/Header.vue'
  import Footer from '~/components/Footer.vue'

  export default {
    components: {
      Header,
      Footer
    }
  }
</script>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

#main-container {
  background: #ece9e6; /* fallback for old browsers */
  background: -webkit-linear-gradient(to left, #ece9e6, #ffffff); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(to left, #ece9e6, #ffffff); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
  min-height: 100%;
}
</style>
