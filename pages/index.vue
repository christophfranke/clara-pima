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
    </div>

    <header class="header">
      <div class="left">
        <img class="pima" src="/IMG_0663_PNG.webp" />
      </div>
      <div class="right">
        <img class="name" src="/IMG_0665_PNG.webp" />
        <img class="dots" src="/IMG_0666_PNG.webp" />
      </div>
    </header>

    <div class="main">
      <img class="picture" src="/53892d_efb7351168b34e73a09d86d2ace5a2a1_mv2_d_2000_1333_s_2.webp" />
      <img class="picture" src="/53892d_ca8fffb156274b008d115bb951952bb3_mv2_d_2000_3000_s_2.webp" />
      <img class="picture" src="/53892d_9472e389202344cda0745ee27047eea0_mv2.webp" />
      <img class="picture" src="/53892d_c08330d132e141b4ad5efd1230b2b73e_mv2_d_2000_1333_s_2.webp" />
      <img class="picture" src="/53892d_0abdd849aedd48d7bd2c14ebd6f76339_mv2_d_2028_2881_s_2.webp" />
      <img class="picture" src="/53892d_e55df6c845d84b238a829ba4233d1817_mv2.webp" />
      <img class="picture" src="/53892d_b5d347494572417e8b4d6a5e4d2bbc67_mv2_d_2125_2858_s_2.webp" />
      <div class="book">
        <img class="book-page" src="/53892d_2c490ddb09cc46048c16b27431b54be0_mv2.webp" />
        <div class="book-description">
          <h2 class="book-title">Der blinde Fuchs</h2>
          <h3 class="book-subtitle">und sein magischer Koffer</h3>
        </div>
        <img class="book-page" src="/53892d_01dfd7090f274b8aa970749652dd52a1_mv2.webp" />
        <div />
        <img class="book-page" src="/53892d_a8fa60892753494b8e092ebaed225a71_mv2.webp" />
      </div>
    </div>

    <div class="about">
      <div class="left">
        <img class="profile" src="/_DSF0046.jpg" />
      </div>
      <div class="right">
        <h2 class="clara">Clara Haseloff</h2>
        <p class="description">artist, author, photograph and yoga teacher, living in Berlin.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
body {
  background-color: #171717;
  color: white;
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


.main {
  margin-top: -225px;
}

.picture {
  border: 3px solid #fff;
  display: block;
  margin: 300px auto;
  max-width: calc(100% - 6px);
  height: auto;
  max-height: 80vh;
}

.book {
  display: grid;
  grid-gap: 0;
  grid-template-columns: 1fr 1fr 1fr;
}

.book-page {
  width: 100%
}

.book-description {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

@font-face {
  font-family: 'Consola';
  src: url('/CONSOLA.TTF') format('truetype');
}

.book-title {
  font-family: 'Consola', monospace;
  font-weight: normal;
  text-align: center;
  font-size: 40px;
  margin: 0;
}
.book-subtitle {
  font-family: 'Consola', monospace;
  font-weight: normal;
  text-align: center;
  font-size: 24px;
  margin-top: 20px;
}

.about {
  margin-top: 400px;  
  display: flex;
  justify-content: space-between;
  align-items: stretch;

  .left, .right {
    width: calc(50% - 8px);
  }

  .right {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .profile {
    width: 100%;
  }

  .clara {
    font-family: 'Consola', monospace;
    font-weight: normal;
    text-align: left;
    font-size: 40px;
    margin: 0;
  }
  .description {
    font-family: 'Consola', monospace;
    font-weight: normal;
    font-style: italic;
    text-align: left;
    font-size: 24px;
    margin-top: 20px;
  }
}

</style>