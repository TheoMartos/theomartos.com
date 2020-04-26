<template>
  <div id="header" class="pt-4 row">
    <div class="mx-auto text-center">
      <a href="/"><b-img src="imgs/pp.png" alt="Profile picture" rounded="circle" height="200px" class="mb-2"></b-img></a>
      <h1>Théo Martos</h1>
    </div>
    <navigation-bar />
  </div>
</template>

<script>
  import NavigationBar from './NavigationBar.vue';

  export default {
    components: {
      NavigationBar
    }
  }

</script>

<style>
  #header {
    /* color: #35495e; */
    background-color: #343a40;
  }

  #header div h1 {
    color: white;
  }
</style>