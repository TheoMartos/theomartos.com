<template>
  <b-nav-item :active="active" :disabled="disabled" :href="href">{{ title }}</b-nav-item>
</template>

<script>
  export default {
    name: 'NavigationItem',
    props: {
      active: false,
      disabled: false,
      title: String,
      href: String
    }
  }
</script>
