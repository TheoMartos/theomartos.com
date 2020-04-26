<template>
  <footer class="row">
      <div class="container d-flex align-items-center justify-content-center">
        <span>&copy; {{ year }} Théo Martos - Published under the Apache 2 licence</span>
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
</style>