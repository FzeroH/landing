<template>
  <div class="social-networks">
    <nuxt-link  v-for="(image, index) in images" :key="index" :to="`/${ image.networkName }`">
      <img :src="require(`assets/images/social_networks_white/${image.src}`)" :alt="`${ image.networkName }`"/>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'SocialNetwork',
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
  .social-networks {
    display: flex;
    width: 100%;
    justify-content: center;
    align-items: center;
    margin-bottom: 6.25rem;
    a {
      cursor: pointer;
      &:not(:first-child) {
        margin-left: 8.75rem;
      }
    }
    z-index: 1;
  }
</style>
