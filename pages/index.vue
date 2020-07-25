<template>
  <b-container>
    Hi, my name is Théo, I'm a {{ age }} year old engineering student. 
    I'm currently studying at <a href="https://esirem.u-bourgogne.fr">ESIREM</a>, a french engineering school located in Dijon.
    I am learning about IT and networking technologies.
    <br>
    
  </b-container>
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
