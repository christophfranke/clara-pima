<template>
  <footer class="footer">
    <nuxt-link to="/impressum">Impressum</nuxt-link>
    <a href="mailto:mailto:justpima@gmail.com">Kontakt</a>

    <Social />
  </footer>  
</template>

<script>
import Social from '~/components/Social'

export default {
  components: {
    Social,
  }
}
</script>


<style lang="scss" scoped>
.footer {
  margin: 100px 0;
  text-align: center;
  font-size: 20px;

  a {
    color: white;
    text-decoration: none;
    &:hover {
      text-decoration: underline;
    }
  }
}
</style>