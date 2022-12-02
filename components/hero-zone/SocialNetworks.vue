<template>
  <div>
    <nuxt-link  v-for="(image, index) in images" :key="index" :to="`/${ image.networkName }`">
      <img :src="require(`assets/images/social_networks/${image.src}`)" :alt="`${ image.networkName }`">
    </nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'SocialNetworks',
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
}
</script>

<style lang="scss" scoped>
  div {
    margin: 2rem 0;
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
