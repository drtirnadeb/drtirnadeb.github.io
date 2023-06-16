---
layout: page
title: " "
---

<style>
.video-container {
  top: 0;
  leftt: 0;
  height: 100vh;
  width: 100%;
  overflow: hidden;
  z-index: 1;
  margin-bottom: -5px;
}

.video-container video {
  object-fit: cover;
  width: 100%;
  height: 100%;
}

.overlay-text {
  position: absolute;
  top: 70%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 2rem;
  color: white;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
}

.content-wrapper {
  margin-top: 100vh;
  padding: 2rem;
  margin-top: -5px;
}

.column.is-one-quarter {
  float: left;
  margin-right: 1rem;
}

.column:last-child {
  margin-bottom: 1rem;
}

@media screen and (max-width: 768px) {
 .column.is-one-quarter {
   float: none;
   margin-right: 0;
   margin-bottom: 1rem;
  }
}

</style>

<div class="video-container">
  <video autoplay muted loop>
    <source src="/videos/Timelapse_Mt Holyoke_06172020.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  <div class="overlay-text">
    <h3> I am Tirna Deb from India, a seeker of philosophy, ended up in the shores of the Netherlands, trying to unfold the mystery of galactic evolution and the influence of the cosmic environment on the galaxy's structural properties. Besides science; painting, music and poetry accompany me towards the voyage to infinitude. </h3>
  </div>
</div>

