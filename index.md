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

<div id="particles-js"></div>

<div class="overlay-text-2">
  <h4>Specialized in <span id="changing-word">xyz</span>.</h4>
</div>
<script src="particles.js"></script>
<script>
  const changingWord = document.getElementById('changing-word');
  const words = ['galaxy formation and evolution', 'multi-phase gas dynamics of jellyfish galaxies', 'radio astronomy using MeerKAT, ALMA', 'data analysis']; // Add your desired words here
  let index = 0;

  setInterval(() => {
    changingWord.textContent = words[index];
    index = (index + 1) % words.length;
  }, 2000); // Change the duration (in milliseconds) to control the word change frequency

  particlesJS('particles-js', {
    particles: {
      number: {
        value: 80,
        density: {
          enable: true,
          value_area: 800
        }
      },
      color: {
        value: '#ffffff'
      },
      shape: {
        type: 'circle',
        stroke: {
          width: 0,
          color: '#000000'
        },
        polygon: {
          nb_sides: 5
        },
        image: {
          src: 'img/github.svg',
          width: 100,
          height: 100
        }
      },
      opacity: {
        value: 0.5,
        random: false,
        anim: {
          enable: false,
          speed: 1,
          opacity_min: 0.1,
          sync: false
        }
      },
      size: {
        value: 5,
        random: true,
        anim: {
          enable: false,
          speed: 40,
          size_min: 0.1,
          sync: false
        }
      },
      line_linked: {
        enable: true,
        distance: 150,
        color: '#ffffff',
        opacity: 0.4,
        width: 1
      },
      move: {
        enable: true,
        speed: 6,
        direction: 'none',
        random: false,
        straight: false,
        out_mode: 'out',
        attract: {
          enable: false,
          rotateX: 600,
          rotateY: 1200
        }
      }
    },
    interactivity: {
      detect_on: 'canvas',
      events: {
        onhover: {
          enable: true,
          mode: 'repulse'
        },
        onclick: {
          enable: true,
          mode: 'push'
        },
        resize: true
      },
      modes: {
        grab: {
          distance: 400,
          line_linked: {
            opacity: 1
          }
        },
        bubble: {
          distance: 400,
          size: 40,
          duration: 2,
          opacity: 8,
          speed: 3
        },
        repulse: {
          distance: 200,
          duration: 0.4
        },
        push: {
          particles_nb: 4
        },
        remove: {
          particles_nb: 2
        }
      }
    },
    retina_detect: true
  });
</script>
