<template>
  <div>
    <h3>Learn all about me in 60 seconds.</h3>
    <video-player />
  </div>
</template>

<script>
import VideoPlayer from "@/components/about-me/VideoPlayer.vue";

export default {
  name: "AboutMe",
  components: {VideoPlayer}
}
</script>

<style lang="scss" scoped>
  div {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    >h3 {
      font-weight: 400;
      font-size: 2.25rem;
      line-height: 2.7rem;
      margin-bottom: 3.75rem;
    }
  }
</style>
