<template>
  <div class="landing-footer">
    <span>© 2020 Ozart Portfolio Template</span>
    <div class="sn">
      <nuxt-link  v-for="(image, index) in images" :key="index" :to="`/${ image.networkName }`">
        <img :src="require(`assets/images/social_networks_black/${image.src}`)" :alt="`${ image.networkName }`">
      </nuxt-link>
    </div>
  </div>
</template>

<script>
import SocialNetworks from '@/components/SocialNetworks.vue';

export default {
  name: "LandingFooter",
  components: { SocialNetworks },
  data() {
    return {
      images: [
        {
          src: 'facebook.svg',
          networkName: 'facebook'
        },
        {
          src: 'linkedin.svg',
          networkName: 'linkedin'
        },
        {
          src: 'behance.svg',
          networkName: 'behance'
        },
        {
          src: 'twitter.svg',
          networkName: 'twitter'
        },
        {
          src: 'dribbble.svg',
          networkName: 'dribbble'
        }]
    }
  }
}
</script>

<style lang="scss" scoped>
  .landing-footer {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    padding: 200px 32px 0;
  }
  .sn {
    a {
      &:not(:first-child) {
        margin-left: 5rem;
      }
    }
  }
</style>
