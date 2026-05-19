# The HDR Videographic Survey
Future home of the HDR Videographic Survey dataset.

Contact tcanham at yorku dot ca for early access

This work is licensed under a Creative Commons Attribution 4.0 International License.

[![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/)

<style>
  .video-bg-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    overflow: hidden;
    pointer-events: none;
  }
  .video-bg-container video {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
</style>

<div class="video-bg-container">
  <video autoplay muted loop playsinline id="githubBgVideo">
    <source src="your-video-url.mp4" type="video/mp4">
  </video>
</div>

<script>
  // Listens for the video metadata to load before applying the 0.5x speed
  document.getElementById('githubBgVideo').addEventListener('loadedmetadata', function() {
    this.playbackRate = 0.5;
  });
</script>
