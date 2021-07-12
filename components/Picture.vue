<template>
  <div class="picture">
    <img class="image" :src="src" />
    <div class="subtext">
      <span class="title">{{ title }}</span><br />
      <slot />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    src: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
.picture {
  margin: 300px 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.image {
  display: block;
  border: 3px solid #fff;

  max-width: calc(100% - 6px);
  max-height: 80vh;
  height: auto;

  &:hover + .subtext {
    opacity: 1;
  }
}

.title {
  font-size: 24px;
}

.subtext {
  margin-top: 5px;
  will-change: opacity;
  transition: opacity 0.15s;
  white-space: normal;
  opacity: 0;
}
</style>