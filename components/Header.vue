<template>
  <div id="header" class="pt-4 row">
    <div class="mx-auto text-center">
      <a href="/"><b-img src="imgs/pp.png" alt="Profile picture" rounded="circle" height="150px" class="mb-2"></b-img></a>
      <h2>Théo Martos</h2>
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
    background-color: #51555a;
  }

  #header div h2 {
    color: white;
  }
</style>