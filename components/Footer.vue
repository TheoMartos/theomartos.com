<template>
  <footer class="row mt-3">
      <div class="container d-flex align-items-center justify-content-center">
        <span>&copy; {{ year }} Théo Martos - Published under the <a href="https://github.com/TheoMartos/theomartos.com/blob/master/LICENSE">Apache 2.0 licence</a> - <a href="/legals">Legals</a></span>
      </div>
  </footer>
</template>

<script>
  export default {
    name: 'Footer',
    computed: {
      year: () => {
        return (new Date).getFullYear();
      }
    }
  }
</script>

<style>
footer {
  background-color: #343a40;
  color: white;
  min-height: 50px;
}

footer div span a, footer div span a:hover, footer div span a:visited {
  color: white;
  text-decoration: underline;
}
</style>