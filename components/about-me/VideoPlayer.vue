<template>
  <div>
    <video src="@/assets/video.mp4" ref="video"
           @pause="pauseVideo" />
    <img src="@/assets/images/play-button.svg"
         alt="play-button"
         v-if="!played"
         @click="playVideo">
  </div>
</template>

<script>
export default {
  name: "VideoPlayer",
  data() {
    return {
      played: false,
    }
  },

  mounted() {
    this.$refs.video.controls = false;
  },
  methods: {
    playVideo() {
        this.$refs.video.play();
        this.$refs.video.controls = true;
        this.played = !this.played
    },
    pauseVideo() {
      this.played = !this.played
      this.$refs.video.controls = false;
    }
  },
}
</script>

<style lang="scss" scoped>
  div {
    position: relative;
    width: 78.9rem;
    height: 44.7rem;

    video {
      width: 100%;
      height: 100%;
    }

    img {
      position: absolute;
      margin: auto;
      max-width: 80px;
      max-height: 80px;
      border-radius: 50%;

      &:hover {
        cursor: pointer;
      }
    }
  }
</style>
