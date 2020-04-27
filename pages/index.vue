<template>
  <section class="container">

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
