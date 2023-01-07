<template>
  <div class="contact">
    <h1>Hello</h1>
    <p>Get in touch</p>
    <h2>Just Say Hello!</h2>
    <button>Contact</button>
    <social-network/>
  </div>
</template>

<script>
import SocialNetwork from "./SocialNetwork.vue";

export default {
  name: 'Contact',
  components: {SocialNetwork}
}
</script>

<style lang="scss" scoped>
  .contact {
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: #333333;
    width: 100%;
    height: fit-content;
    h1 {
      position: absolute;
      left: calc(50% - 1279px/2 + 0.5px);
      top: 0.9rem;
      font-weight: 400;
      font-size: 28rem;
      line-height: 33.2rem;
      letter-spacing: 0.1em;
      color: #3A3A3A;
      &:hover {
        cursor: default;
      }
    }
    p, h2{
      color: #ffffff;
      font-weight: 400;
      z-index: 1;
    }
    p {
      font-size: 2rem;
      line-height: 2.375rem;
      margin-top: 6.25rem;
    }
    h2 {
      margin-top: 1.5rem;
      font-size: 3.375rem;
      line-height: 4rem;
    }
    button {
      margin: 5rem 0;
      padding: 1.25rem 2.5rem;
      font-weight: 400;
      font-size: 1.75rem;
      line-height: 2rem;
      color: #363434;
      z-index: 1;
      &:hover {
        cursor: pointer;
      }
    }
  }
</style>
