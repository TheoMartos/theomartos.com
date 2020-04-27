<template>
  <b-card :img-alt=social :img-src=imgSrc img-left class="pl-3 mx-3 my-3 social-card">
    <b-card-text class="text-center">
      <a :href=href >{{ content }}</a>
    </b-card-text>
  </b-card>
</template>

<script>
export default {
  name: 'Social',
  props: {
    img: String,
    social: String,
    content: String,
    href: String
  },
  computed: {
    imgSrc() {
      return 'imgs/' + this.img
    }
  }
}
</script>

<style>
  .social-card {
    min-width: 150px;
  }
</style>