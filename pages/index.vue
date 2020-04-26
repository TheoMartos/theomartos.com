<template>
  <section class="container mt-4">
    <p>
      Hi! I am a {{ age }} years old engineering student studing at <a href="https://esirem.u-bourgogne.fr">ESIREM</a>,
      Dijon, France.
    </p>
  </section>
</template>

<script>
  export default {
    computed: {
      age: () => {
        const birthday = new Date('November 7, 1998');
        const diff = new Date(Date.now() - birthday);

        return diff.getUTCFullYear() - 1970;
      }
    }
  }
</script>
