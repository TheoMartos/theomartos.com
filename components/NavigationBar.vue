<template>
  <b-navbar id="nav-bar" type="dark" variant="dark" class="justify-content-center">
    <b-navbar-nav>
      <navigation-item title="About" href="/" active />
      <navigation-item title="Schooling" href="/schooling" />
      <navigation-item title="Projects" href="/projects" />
      <navigation-item title="Social Medias" href="/socials" />
      <navigation-item title="Contact" href="/contact" />
    </b-navbar-nav>
  </b-navbar>
</template>

<script>
  import NavigationItem from './NavigationItem.vue';

  export default {
    name: 'NavigationBar',
    components: {
      NavigationItem
    }
  }
</script>

<style>
#nav-bar {
  width: 100%;
}
</style>