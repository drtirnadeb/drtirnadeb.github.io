---
layout: page
title: " "
---

<style>
.video-container {
  top: 0;
  left: 0;
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
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 2rem;
  color: white;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
}

.overlay-text-2 {
  position: absolute;
  top: 80%;
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
    <h4>I am Tirna Deb, a seeker of philosophy</h4>
  </div>
</div>
<div class="overlay-text-2">
  <h4>Specialized in <span id="changing-word">xyz</span>.</h4>
</div>
<br>
<p>
  I am Tirna Deb, a PhD in astronomy, experienced in statistical data processing, programming, and modelling. During my PhD in the Netherlands, I investigated the mystery of galactic evolution and the influence of the cosmic environment on the galaxy's structural properties. After obtaining a prestigious fellowship to conduct independent research, I am currently conducting research as the principal investigator (PI) of a project that I designed myself. I am also visiting several universities in the USA to broaden my collaboration and my scientific horizons. Though I am originally from India, I have lived and worked on four different continents. Thus, I consider myself a global citizen, a person with a unique combination of openness to new ideas and a strong hold on their own ideals and roots.

</p>
<script>
  const changingWord = document.getElementById('changing-word');
  const words = ['galaxy formation and evolution', 'multi-phase gas dynamics of jellyfish galaxies', 'radio astronomy using MeerKAT, ALMA', 'data analysis']; // Add your desired words here
  let index = 0;

  setInterval(() => {
    changingWord.textContent = words[index];
    index = (index + 1) % words.length;
  }, 2000); // Change the duration (in milliseconds) to control the word change frequency
});
</script>
