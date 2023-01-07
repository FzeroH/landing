<template>
  <div>
    <Header />
    <hero-zone @scroll-to="scrollTo()"/>
    <about-me />
    <what-i-do />
    <contact />
  </div>
</template>

<script>
import Contact from "../components/contact/Contact.vue";

export default {
  name: 'IndexPage',
  components: {Contact},
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
