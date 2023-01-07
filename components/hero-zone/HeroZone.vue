<template>
  <div class="hero__zone">
    <div class="hero__container">
      <section class="hero__container-inf">
        <span>Hello</span>
        <h2>I'm Sarah Jackson</h2>
        <p>A UX / UI designer, product designer, content creator and creative director.</p>
        <p>Of course, there’s so much more to me than just a few fancy titles. Scroll down and get to know me.</p>
      </section>
      <img src="@/assets/images/ImageContainer.png" alt="image">
    </div>
    <social-networks @scroll-to="$emit('scroll-to')" />
  </div>
</template>

<script>
import SocialNetworks from "@/components/SocialNetworks.vue";

export default {
  name: 'HeroZone',
  components: {SocialNetworks}
}
</script>

<style lang="scss" scoped>
.hero__zone {
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin-bottom: 7.3rem;
}

.hero__container {
  display: flex;

  >img {
    max-width: 34.4rem;
    max-height: 40rem;
  }
}
.hero__container-inf {
  padding-left: 2rem;
  padding-right: 3.5rem;
  > h2, p {
    padding-top: 20px;
  }
  span {
    position: relative;
    padding-left: 3.8rem;
    font-weight: 700;
    font-size: 2.1rem;
    line-height: 2.44rem;
    &::before {
      position: absolute;
      top: 50%;
      left: 0;
      content: '';
      width: 3rem;
      height: 2px;
      background: #333333;
    }
  }

  h2 {
    font-weight: 500;
    font-size: 4.6rem;
    line-height: 5.5rem;
  }

  p {
    &:nth-child(3) {
      font-size: 2.5rem;
      line-height: 2.9rem;
    }

    &:nth-child(4) {
      font-size: 1.5rem;
      line-height: 1.7rem;
    }
  }
}

</style>
