<template>
  <span class="arrow">
  </span>
</template>

<script>
export default {
  name: 'Arrow'
}
</script>

<style lang="scss" scoped>
  .arrow, .arrow::before, .arrow::after {
    position: absolute;
    right: 0;
    background-color: #fff;
    width: 42px;
    &::before {
      transform: rotate(45deg);
    }
    &::after {
      transform: rotate(-45deg);
    }
  }
</style>
