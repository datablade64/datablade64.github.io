---
layout: default
title: datablade64
---

<main class="shell">
  <header class="banner">
    <div class="hero-card">
      <div class="hero-bar">
        <span class="bar-dot red"></span>
        <span class="bar-dot yellow"></span>
        <span class="bar-dot green"></span>
        <span class="bar-title">datablade64 — ai × embedded</span>
      </div>

      <div class="hero-body">
        <svg viewBox="0 0 900 400" xmlns="http://www.w3.org/2000/svg" class="hero-svg" preserveAspectRatio="xMidYMid slice" role="img" aria-label="circuit board and neural network">
          <defs>
            <linearGradient id="bgGrad" x1="0%" y1="0%" x2="0%" y2="100%">
              <stop offset="0%" stop-color="#0b0c10"/>
              <stop offset="100%" stop-color="#07080a"/>
            </linearGradient>
            <radialGradient id="vignette" cx="50%" cy="50%" r="65%">
              <stop offset="0%" stop-color="#07080a" stop-opacity="0.95"/>
              <stop offset="100%" stop-color="#07080a" stop-opacity="0"/>
            </radialGradient>
          </defs>

          <rect width="900" height="400" fill="url(#bgGrad)"/>

          <!-- grid -->
          <g stroke="#131519" stroke-width="1">
            <line x1="0" y1="80" x2="900" y2="80"/>
            <line x1="0" y1="200" x2="900" y2="200"/>
            <line x1="0" y1="320" x2="900" y2="320"/>
            <line x1="180" y1="0" x2="180" y2="400"/>
            <line x1="450" y1="0" x2="450" y2="400"/>
            <line x1="720" y1="0" x2="720" y2="400"/>
          </g>

          <!-- data path across center (behind text) -->
          <path class="trace" d="M 265 200 L 635 200" stroke="#00ff9d" stroke-width="2" fill="none" opacity="0.15"/>

          <!-- LEFT: PCB -->
          <g id="pcb">
            <rect x="15" y="40" width="250" height="320" fill="none" stroke="#1e2229" stroke-width="2" rx="8"/>
            <circle cx="28" cy="53" r="5" fill="none" stroke="#1e2229" stroke-width="1.5"/>
            <circle cx="252" cy="53" r="5" fill="none" stroke="#1e2229" stroke-width="1.5"/>
            <circle cx="28" cy="347" r="5" fill="none" stroke="#1e2229" stroke-width="1.5"/>
            <circle cx="252" cy="347" r="5" fill="none" stroke="#1e2229" stroke-width="1.5"/>

            <!-- silkscreen -->
            <rect x="35" y="55" width="70" height="30" fill="none" stroke="#1a1d25" stroke-width="1.5" rx="3"/>

            <!-- traces -->
            <g stroke="#00ff9d" stroke-width="3" fill="none" stroke-linecap="round">
              <path class="trace" d="M 35 110 L 72 110 L 72 170"/>
              <path class="trace" d="M 35 330 L 60 330 L 60 230 L 72 230"/>
              <path class="trace" d="M 245 95 L 220 95 L 220 170 L 208 170"/>
              <path class="trace" d="M 245 315 L 220 315 L 220 230 L 208 230"/>
            </g>

            <!-- vias -->
            <g fill="#00ff9d">
              <circle cx="35" cy="110" r="4"/>
              <circle cx="35" cy="330" r="4"/>
              <circle cx="245" cy="95" r="4"/>
              <circle cx="245" cy="315" r="4"/>
              <circle cx="140" cy="310" r="3.5"/>
              <circle cx="140" cy="90" r="3.5"/>
            </g>

            <!-- chip -->
            <g transform="translate(140,200)">
              <rect x="-55" y="-45" width="110" height="90" fill="#0e1116" stroke="#00ff9d" stroke-width="2" rx="6"/>
              <rect x="-45" y="-35" width="90" height="70" fill="none" stroke="#00ff9d" stroke-width="0.8" rx="3" opacity="0.4"/>
              <circle cx="38" cy="-30" r="4" fill="none" stroke="#00ff9d" stroke-width="1.5"/>
              <line x1="-55" y1="-30" x2="-68" y2="-30" stroke="#00ff9d" stroke-width="1.5"/>
              <line x1="-55" y1="-10" x2="-68" y2="-10" stroke="#00ff9d" stroke-width="1.5"/>
              <line x1="-55" y1="10" x2="-68" y2="10" stroke="#00ff9d" stroke-width="1.5"/>
              <line x1="-55" y1="30" x2="-68" y2="30" stroke="#00ff9d" stroke-width="1.5"/>
              <line x1="55" y1="-30" x2="68" y2="-30" stroke="#00ff9d" stroke-width="1.5"/>
              <line x1="55" y1="-10" x2="68" y2="-10" stroke="#00ff9d" stroke-width="1.5"/>
              <line x1="55" y1="10" x2="68" y2="10" stroke="#00ff9d" stroke-width="1.5"/>
              <line x1="55" y1="30" x2="68" y2="30" stroke="#00ff9d" stroke-width="1.5"/>
            </g>
          </g>

          <!-- RIGHT: Neural network -->
          <g id="nn">
            <rect x="630" y="55" width="255" height="290" fill="none" stroke="#1e2229" stroke-width="2" rx="8"/>

            <!-- connections input -> hidden -->
            <g stroke="#00ff9d" stroke-width="0.9" opacity="0.35">
              <line class="nline" x1="670" y1="130" x2="755" y2="110"/>
              <line class="nline" x1="670" y1="130" x2="755" y2="155"/>
              <line class="nline" x1="670" y1="130" x2="755" y2="200"/>
              <line class="nline" x1="670" y1="170" x2="755" y2="110"/>
              <line class="nline" x1="670" y1="170" x2="755" y2="155"/>
              <line class="nline" x1="670" y1="170" x2="755" y2="200"/>
              <line class="nline" x1="670" y1="170" x2="755" y2="245"/>
              <line class="nline" x1="670" y1="210" x2="755" y2="155"/>
              <line class="nline" x1="670" y1="210" x2="755" y2="200"/>
              <line class="nline" x1="670" y1="210" x2="755" y2="245"/>
              <line class="nline" x1="670" y1="210" x2="755" y2="290"/>
              <line class="nline" x1="670" y1="250" x2="755" y2="200"/>
              <line class="nline" x1="670" y1="250" x2="755" y2="245"/>
              <line class="nline" x1="670" y1="250" x2="755" y2="290"/>
            </g>

            <!-- connections hidden -> output -->
            <g stroke="#00ff9d" stroke-width="0.9" opacity="0.35">
              <line class="nline" x1="755" y1="110" x2="835" y2="150"/>
              <line class="nline" x1="755" y1="110" x2="835" y2="200"/>
              <line class="nline" x1="755" y1="155" x2="835" y2="150"/>
              <line class="nline" x1="755" y1="155" x2="835" y2="200"/>
              <line class="nline" x1="755" y1="155" x2="835" y2="250"/>
              <line class="nline" x1="755" y1="200" x2="835" y2="150"/>
              <line class="nline" x1="755" y1="200" x2="835" y2="200"/>
              <line class="nline" x1="755" y1="200" x2="835" y2="250"/>
              <line class="nline" x1="755" y1="245" x2="835" y2="200"/>
              <line class="nline" x1="755" y1="245" x2="835" y2="250"/>
              <line class="nline" x1="755" y1="290" x2="835" y2="250"/>
              <line class="nline" x1="755" y1="290" x2="835" y2="200"/>
            </g>

            <!-- nodes: input -->
            <g fill="#00ff9d">
              <circle class="node" cx="670" cy="130" r="5.5"/>
              <circle class="node" cx="670" cy="170" r="5.5" style="animation-delay:0.4s"/>
              <circle class="node" cx="670" cy="210" r="5.5" style="animation-delay:0.8s"/>
              <circle class="node" cx="670" cy="250" r="5.5" style="animation-delay:1.2s"/>
            </g>
            <!-- nodes: hidden -->
            <g fill="#00ff9d">
              <circle class="node" cx="755" cy="110" r="5.5" style="animation-delay:0.2s"/>
              <circle class="node" cx="755" cy="155" r="5.5" style="animation-delay:0.6s"/>
              <circle class="node" cx="755" cy="200" r="5.5" style="animation-delay:1s"/>
              <circle class="node" cx="755" cy="245" r="5.5" style="animation-delay:1.4s"/>
              <circle class="node" cx="755" cy="290" r="5.5" style="animation-delay:1.8s"/>
            </g>
            <!-- nodes: output -->
            <g fill="#00ff9d">
              <circle class="node" cx="835" cy="150" r="6.5" style="animation-delay:0.5s"/>
              <circle class="node" cx="835" cy="200" r="6.5" style="animation-delay:0.9s"/>
              <circle class="node" cx="835" cy="250" r="6.5" style="animation-delay:1.3s"/>
            </g>
          </g>

          <!-- darken center so text pops -->
          <rect width="900" height="400" fill="url(#vignette)"/>
        </svg>

        <div class="hero-text">
          <h1>datablade64</h1>
          <p class="subtitle">AI <span class="dot">·</span> Embedded Systems</p>
          <div class="status">&gt; coming soon<span class="cursor">▌</span></div>
        </div>
      </div>
    </div>
  </header>

  <section class="intro">
    <p>Coming soon: AI and embedded systems projects.</p>
  </section>
</main>
