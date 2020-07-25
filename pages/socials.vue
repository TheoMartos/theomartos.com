<template>
  <b-container>
    <h4 class="text-center">You can find me here</h4>
    <div id="socials" class="d-flex justify-content-center">
      <div>
        <social href="https://github.com/TheoMartos" content="TheoMartos" img="github.svg" social="Github" />
        <social href="https://gitlab.com/theo.martos" content="@theo.martos" img="gitlab.svg" social="Gitlab" />
      </div>
      <div>
        <social href="https://www.linkedin.com/in/th%C3%A9o-martos-52734a172/" content="Théo Martos" img="linkedin.svg" social="Linkedin" />
        <social href="https://twitter.com/theo__martos" content="@theo__martos" img="twitter.svg" social="Twitter" />
      </div>
    </div>
  </b-container>
</template>

<script>
import Social from "~/components/Social.vue";

export default {
  components: {
    Social
  }
}
</script>