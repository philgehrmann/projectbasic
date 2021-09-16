<template>
  <div id="app" >
    <div id="video-wrapper" class="startscreen">
      <video width="100%" height="100%" autoplay style="pointer-events: none;">
      <source src="../assets/video.mp4" type="video/mp4">
</video>
    </div>
    <Header />
    <div class="content-intro p-10 container mx-auto border-2">

    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style lang="scss">
  body {
    background: rgb(19, 19, 19);
    color: #fff;
  }
  .content-intro {
    height: 85vh;
  }

  .startscreen {
    position: absolute;
    overflow:hidden;
    z-index:-1;
    top:0;
    bottom:0;
    width: 100%;
    height: 100vh;

    video {
      opacity: .1;
    }
  }
</style>
