<template>
  <div>
    <div class="social">
      <a class="link" href="https://www.facebook.com/Pimamip" target="_blank">
        <svg class="facebook" viewBox="0 30 448 450">
          <use xlink:href="/facebook.svg#icon" />
        </svg>
      </a>
      <a class="link" href="https://www.instagram.com/daspima/" target="_blank">
        <img class="instagram hover" src="/instagram.svg">
        <img class="instagram white" src="/instagram-white.svg">
      </a>
      <a class="link" href="mailto:justpima@gmail.com" target="_blank">
        <svg class="email" viewBox="0 0 512 512">
          <use xlink:href="/email.svg#icon" />
        </svg>
      </a>
    </div>

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
  </div>
</template>

<style>
body {
  background-color: #171717;
  color: white;

  font-family: 'Consola', monospace;
  font-weight: normal;
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
    transform: translate(100%, -50%);
  }
}

.social {
  margin-top: 40px;
  display: flex;
  justify-content: center;
  align-items: center;

  .link {
    margin: 0 4px;
  }

}

.facebook {
  height: 32px;
  color: white;
  a:hover & {
    background-color: white;
    background: linear-gradient(90deg, rgba(0,0,0,0) 0%, rgba(255,255,255,1) 10%, rgba(255,255,255,1) 90%, rgba(0,0,0,0) 100%);
    color: #3b5998;
  }
}

.instagram {
  height: 40px;
  width: auto;

  &.hover {
    display: none;
  }

  a:hover & {
    display: none;
    &.hover {
      display: inline-block;
    }
  }
}

.email {
  height: 36px;
  padding: 0 5px;
  margin: 0 -5px;
  color: white;
  a:hover & {
    background-color: white;
    color: black;
  }
}
</style>