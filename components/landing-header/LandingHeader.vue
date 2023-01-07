<template>
  <header class="landing__header">
    <img src="@/assets/images/logo.svg" alt="logo" class="landing__header-logo"/>
    <img src="@/assets/images/search.svg" alt="search" class="landing__header-search"/>
    <div>
      <a href="/">Menu</a>
    </div>
  </header>
</template>

<script>

export default {
  name: 'Header',
}
</script>

<style lang="scss" scoped>
  .landing__header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 2rem;

    .landing__header-logo {
      max-width: 10.9rem;
      max-height: 4rem;
    }

    .landing__header-search {
      max-width: 2rem;
      max-height: 2rem;
    }
    div {
      display: flex;
      align-items: center;
      position: relative;

      a {
        font-weight: 300;
        font-size: 1.5rem;
        line-height: 1.75rem;
      }
    }
  }
</style>
