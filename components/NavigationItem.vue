<template>
  <b-nav-item :active="active" :disabled="disabled" :href="href">{{ title }}</b-nav-item>
</template>

<script>
  export default {
    name: 'NavigationItem',
    data() {
      return { active: false }
    },
    props: {
      disabled: false,
      title: String,
      href: String
    },
    created() {
      this.active = this.$route.path.endsWith(this.href)
    }
  }
</script>

<style scoped>
li {
  font-size: 1.15em;
}
</style>