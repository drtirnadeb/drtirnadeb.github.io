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
  text-align: center; /* Added to center-align the text */
}

.overlay-text-2 {
  position: absolute;
  top: 80%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 2rem;
  color: white;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
  text-align: center; /* Added to center-align the text */
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
    <h4>I am Tirna Deb</h4>
  </div>
</div>
<div class="overlay-text-2">
  <h4>Specialized in <span id="changing-word"></span></h4>
</div>
<br>
<p>
I am Tirna Deb, a PhD in Astrophysics, experienced in data-driven research, statistical data reduction, processing, modeling, machine learning, and programming. My expertise includes <strong>detecting faint signals, handling high-dimensional and noisy datasets, anomaly detection, and data visualization</strong>. I enjoy <strong>diving deep into complex datasets, uncovering hidden patterns, and translating raw data into meaningful discoveries with real-world impact</strong>. While my background is in astronomical research—studying galaxy evolution and radio astronomy—my expertise lies in extracting insights from complex datasets. During my PhD in the Netherlands, I investigated the mystery of galactic evolution and how the cosmic environments shape galaxy structures, applying advanced data analysis techniques along the way.

After receiving the prestigious Rubicon fellowship, I moved to <strong>Harvard University</strong> to lead my own independent research as the principal investigator (PI) of a project I designed. As I navigate the intersection of <strong>data science, machine learning, and scientific research</strong>, I am actively working toward expanding my collaborations and broadening my expertise beyond academia.

Though originally from India, I have lived and worked across four continents, shaping my perspective as a global citizen—open to new ideas while staying deeply connected to my roots.
</p>
<script>
  const changingWord = document.getElementById('changing-word');
  const words = ['Statistical Data Processing', 'Anomaly Detection & Signal Processing', 'Programming (Python)', 'Machine Learning & Data Science', 'Radio astronomy', 'Galaxy evolution']; // Add your desired words here
  let index = 0;

  setInterval(() => {
    changingWord.innerHTML = '<span style="color: #FF8C00">' + words[index] + '</span>'; // Wrap changing word in a span with the desired color
    index = (index + 1) % words.length;
  }, 2000); // Change the duration (in milliseconds) to control the word change frequency
</script>
