<template>
  <div>
    <Header />
    <hero-zone @scroll-to="scrollTo()"/>
    <about-me />
    <what-i-do />
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  methods: {
    scrollTo(){
      window.scroll({
        left: 0,
        top: 969,
        behavior: 'smooth',
      })
    },
  },
}
</script>
