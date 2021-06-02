<template>
  <div>
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
        <div />
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

    <footer class="footer">
      <nuxt-link to="/impressum">Impressum</nuxt-link>
      <a href="mailto:mailto:justpima@gmail.com">Kontakt</a>
    </footer>
  </div>
</template>

<script>
export default {

}
</script>


<style lang="scss" scoped>
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

  > * {
    width: 100%;
    border-bottom: 3px solid white;

    &:nth-last-child(1),
    &:nth-last-child(2),
    &:nth-last-child(3) {
      border-bottom: none;
    }
    &:nth-child(3n + 2) {
      width: calc(100% - 6px);
      border-right: 3px solid white;
      border-left: 3px solid white;
    }
  }
}

.book-description {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.book-title {
  text-align: center;
  font-size: 40px;
  margin: 0;
}
.book-subtitle {
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