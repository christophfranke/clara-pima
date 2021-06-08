<template>
  <div>
    <Social />

    <header class="header">
      <div class="left">
        <nuxt-link to="/">
          <img class="pima" src="/IMG_0663_PNG.webp" />
        </nuxt-link>
      </div>
      <div class="right">
        <img class="name" src="/IMG_0665_PNG.webp" />
        <img class="dots" src="/IMG_0666_PNG.webp" />
      </div>
    </header>

    <nuxt/>

    <Footer />
  </div>
</template>

<script>
import Social from '~/components/Social'
import Footer from '~/components/Footer'

export default {
  components: {
    Social,
    Footer,
  }
}
</script>

<style>
body {
  background-color: #280038;
  background-color: #1a0024;
  background-color: #ff0095;
  background-color: #171717;
  color: white;

  font-family: 'Consola', monospace;
  font-weight: normal;
}

a, a:visited {
  color: white;
}

@font-face {
  font-family: 'Consola';
  src: url('/CONSOLA.TTF') format('truetype');
}
</style>

<style lang="scss" scoped>
.header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  pointer-events: none;

  display: flex;
  justify-content: space-between;
  align-items: flex-start;

  .left {
    width: 400px;
    pointer-events: auto;
  }

  .pima {
    width: 100%;
    -webkit-filter: grayscale(1) invert(1);
    filter: grayscale(1) invert(1);
  }

  .right {
    width: 400px;
  }

  .name {
    display: block;
    width: 100%;
    -webkit-filter: grayscale(1) invert(1);
    filter: grayscale(1) invert(1);
  }

  .dots {
    width: 50%;
    -webkit-filter: grayscale(1) invert(1);
    filter: grayscale(1) invert(1);
    transform: translate(85%, -60%);
  }
}
</style>