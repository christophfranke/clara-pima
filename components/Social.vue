<template>
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
</template>

<style lang="scss" scoped>
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