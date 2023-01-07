<template>
  <div>
    <nuxt-link  v-for="(image, index) in images" :key="index" :to="`/${ image.networkName }`">
      <img :src="require(`assets/images/social_networks_black/${image.src}`)" :alt="`${ image.networkName }`">
    </nuxt-link>
    <scroll-button @scroll-to="$emit('scroll-to')"/>
  </div>
</template>

<script>
import ScrollButton from '@/components/hero-zone/ScrollButton.vue';

export default {
  name: 'SocialNetworks',
  components: { ScrollButton },
  data() {
    return {
      images: [
        {
        src:'facebook.svg',
        networkName:'facebook'
        },
        {
        src:'linkedin.svg',
        networkName:'linkedin'
        },
        {
        src:'behance.svg',
        networkName:'behance'
        },
        {
        src:'twitter.svg',
        networkName:'twitter'
        },
        {
        src:'dribbble.svg',
        networkName:'dribbble'
        }]
    }
  },
  methods: {
    test() {
      this.$emit('scroll-to')
    }
  },
}
</script>

<style lang="scss" scoped>
  div {
    display: flex;
    flex-direction: row;
    max-height: fit-content;
    margin: 2rem 0;
    position: relative;
    a {
      position: relative;
      margin-left: 1rem;
      width: 1.25rem;
      height: 1.25rem;
      img {
        max-width: 100%;
        max-height: 100%;
      }
    }
  }
</style>
