<template>
  <div class="scroll__button" @click="$emit('scroll-to')">
    <span class="scroll__button-title">
      Scroll
    </span>
    <img src="@/assets/images/arrow.svg" class="scroll__button-arrow">
  </div>
</template>

<script>
export default {
  name: "ScrollButton"
}
</script>

<style lang="scss" scoped>
  .scroll__button {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 0;
    position: absolute;
    top: 0;
    left: 50%;
    &:hover {
      cursor: pointer;
    }
  }
  .scroll__button-title {
    font-family: 'Rubik', sans-serif;
    font-style: normal;
    font-weight: 300;
    font-size: 1.125rem;
    line-height: 1.3;
    text-transform: uppercase;
  }
  .scroll__button-arrow {
    max-width: 1rem;
    max-height: 2rem;
  }
</style>
