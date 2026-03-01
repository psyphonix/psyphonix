<div align="center">
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&display=swap');

    .cyber-container {
      font-family: 'Orbitron', sans-serif;
      position: relative;
      background-color: #0d0d0d;
      color: #00ffcc;
      padding: 20px;
      border: 2px solid #00ffcc;
      border-radius: 15px;
      box-shadow: 0 0 20px #00ffcc, inset 0 0 20px #00ffcc;
      text-align: left;
      max-width: 800px;
      margin: auto;
      overflow: hidden; /* To contain the animation */
    }

    .background-animation {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
    }

    .particle {
      position: absolute;
      background-color: #6eff3e;
      opacity: 0;
      z-index: 1;
      animation: rain-fall 5s infinite linear, particle-flicker 2s infinite alternate;
    }

    @keyframes rain-fall {
      0% {
        transform: translateY(-10vh);
        opacity: 0;
      }
      10% {
        opacity: 1;
      }
      90% {
        opacity: 1;
      }
      100% {
        transform: translateY(100vh);
        opacity: 0;
      }
    }
    
    @keyframes particle-flicker {
        0%, 100% { opacity: 1; }
        50% { opacity: 0.5; }
    }

    .warp-core {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 150px;
        height: 150px;
        background: radial-gradient(circle, #ffffff 0%, #add8e6 30%, #00ffff 60%, rgba(0, 255, 255, 0) 70%);
        border-radius: 50%;
        z-index: 2;
        animation: pulsate-glow 3s infinite ease-in-out;
    }

    @keyframes pulsate-glow {
        0% {
            transform: translate(-50%, -50%) scale(1);
            box-shadow: 0 0 20px #00ffff, 0 0 30px #00ffff, 0 0 40px #00ffff;
        }
        50% {
            transform: translate(-50%, -50%) scale(1.1);
            box-shadow: 0 0 30px #ffffff, 0 0 40px #ffffff, 0 0 50px #ffffff;
        }
        100% {
            transform: translate(-50%, -50%) scale(1);
            box-shadow: 0 0 20px #00ffff, 0 0 30px #00ffff, 0 0 40px #00ffff;
        }
    }

    .content-wrapper {
        position: relative;
        z-index: 3;
    }

    .cyber-header {
      text-align: center;
      font-size: 2.5em;
      font-weight: 700;
      text-shadow: 0 0 10px #00ffcc, 0 0 20px #00ffcc;
      animation: flicker 1.5s infinite alternate;
    }

    @keyframes flicker {
      0%, 100% {
        text-shadow: 0 0 10px #00ffcc, 0 0 20px #00ffcc;
        opacity: 1;
      }
      50% {
        text-shadow: 0 0 5px #00ffcc, 0 0 10px #00ffcc;
        opacity: 0.8;
      }
    }

    .cyber-section-title {
      font-size: 1.8em;
      color: #6eff3e;
      text-shadow: 0 0 8px #6eff3e;
      border-bottom: 2px solid #6eff3e;
      padding-bottom: 5px;
      margin-top: 30px;
    }

    .cyber-text {
      font-size: 1em;
      line-height: 1.6;
    }

    .cyber-list {
      list-style-type: none;
      padding-left: 0;
    }

    .cyber-list-item {
      border: 1px solid #48fdd9;
      text-emphasis-color: #ffffff;
      background-color: #1a1a1a;
      border: 1px solid #48fdd9;
      border-left: 5px solid #6eff3e;
      padding: 10px;
      margin-bottom: 10px;
      border-radius: 5px;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .cyber-list-item:hover {
      transform: scale(1.02);
      box-shadow: 0 0 15px #6eff3e;
    }

    .cyber-social-links a {
      color: #6eff3e;
      text-decoration: none;
      font-size: 1.2em;
      margin: 0 15px;
      transition: color 0.3s ease, text-shadow 0.3s ease;
    }

    .cyber-social-links a:hover {
      color: #ffffff;
      text-shadow: 0 0 10px #00ffcc;
    }
  </style>

  <div class="cyber-container">
    <div class="background-animation">
        <div class="warp-core"></div>
    </div>
    <div class="content-wrapper">
        <div class="cyber-header">psyphonix</div>
        <br>
        <div class="cyber-text">
        - Welcome to my home page portfolio! This is a place where I showcase my skills, projects, and passions in the world of software for hobby side projects and code tinerking. 
        </div>

        <div class="cyber-section-title">// ABOUT ME</div>
        <div class="cyber-text">
        I am a [Your Role] with a passion for building awesome things. I have experience in a variety of technologies and I am always looking for new challenges.
        </div>

        <div class="cyber-section-title">// SKILLS</div>
        <ul class="cyber-list">
        <li class="cyber-list-item">Languages: [Language 1], [Language 2], [Language 3]</li>
        <li class="cyber-list-item">Frameworks: [Framework 1], [Framework 2], [Framework 3]</li>
        <li class="cyber-list-item">Tools: [Tool 1], [Tool 2], [Tool 3]</li>
        </ul>

        <div class="cyber-section-title">// PROJECTS</div>
        <ul class="cyber-list">
        <li class="cyber-list-item">
            <strong>Project 1:</strong> [Link to Project 1] - A short description of your project.
        </li>
        <li class="cyber-list-item">
            <strong>Project 2:</strong> [Link to Project 2] - A short description of your project.
        </li>
        <li class="cyber-list-item">
            <strong>Project 3:</strong> [Link to Project 3] - A short description of your project.
        </li>
        </ul>

        <div class="cyber-section-title">// CONNECT</div>
        <div class="cyber-social-links" align="center">
        <a href="[Your LinkedIn URL]" target="_blank">LinkedIn</a>
        <a href="[Your Twitter URL]" target="_blank">Twitter</a>
        <a href="[Your Website URL]" target="_blank">Website</a>
        </div>
    </div>
  </div>
  <script>
    const container = document.querySelector('.background-animation');
    for (let i = 0; i < 100; i++) {
      const particle = document.createElement('div');
      particle.classList.add('particle');
      particle.style.left = `${Math.random() * 100}%`;
      particle.style.width = `${Math.random() * 2 + 1}px`;
      particle.style.height = `${Math.random() * 10 + 5}px`;
      particle.style.animationDelay = `${Math.random() * 5}s`;
      particle.style.animationDuration = `${Math.random() * 3 + 2}s`;
      container.appendChild(particle);
    }
  </script>
</div>
