<template>
  <div class="frame">
    <section class="hero-section" data-name="HeroSection">
      <div class="container" data-name="Container">
        <div class="hero-text" data-name="Heading 1">
          <h1 class="title">One Step from Spark to Reality</h1>
          <p class="highlight">NO CAD skill needed</p>
          <p class="description">share your idea freely with Sparkoh using simple words</p>
        </div>

        <div class="action-row">
          <div class="input-box" data-name="HeroSection">
            <p class="placeholder">Describe what you want to create...</p>
            <div class="input-icon" data-name="Icon">
              <svg fill="none" preserveAspectRatio="none" viewBox="0 0 16 16">
                <path
                  d="M8 2V10"
                  stroke="var(--navy)"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="1.33333"
                />
                <path
                  :d="svgPaths.p26e09a00"
                  stroke="var(--navy)"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="1.33333"
                />
                <path
                  :d="svgPaths.p23ad1400"
                  stroke="var(--navy)"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="1.33333"
                />
              </svg>
            </div>
          </div>

          <button class="cta-button" type="button" data-name="Button">
            <svg class="cta-icon" fill="none" preserveAspectRatio="none" viewBox="0 0 20 20">
              <path
                :d="svgPaths.p1a69a80"
                stroke="var(--cream)"
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="1.66667"
              />
              <path
                :d="svgPaths.p136f3380"
                stroke="var(--cream)"
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="1.66667"
              />
            </svg>
            <span>Get Started</span>
          </button>
        </div>
      </div>

      <div class="cube-illustration" data-name="CubeIllustration" aria-hidden="true">
        <div class="cube cube-1"></div>
        <div class="cube cube-2"></div>
        <div class="cube cube-3"></div>
        <div class="cube cube-4"></div>
        <div class="cube cube-5"></div>
        <div class="cube cube-6"></div>
      </div>
    </section>
  </div>
</template>

<script setup>
import svgPaths from '../svg.js';
</script>

<style scoped>
.frame {
  --orange: #ff8361;
  --navy: #003366;
  --cream: #fffbf5;
  --butter: #fff099;
  align-items: center;
  background: var(--cream);
  display: flex;
  justify-content: center;
  min-height: 100%;
  padding: 31px 20px;
}

.hero-section {
  min-height: 366px;
  position: relative;
  width: min(1200px, 100%);
}

.container {
  display: flex;
  flex-direction: column;
  gap: 38px;
  position: relative;
  width: 100%;
  z-index: 2;
}

.hero-text {
  min-height: 165px;
}

.title {
  color: var(--navy);
  font-size: clamp(34px, 4.8vw, 60px);
  font-weight: 700;
  line-height: 1.15;
  margin: 0;
}

.highlight {
  color: var(--orange);
  font-size: clamp(24px, 3.2vw, 36px);
  font-weight: 700;
  line-height: 1.2;
  margin: 8px 0 0;
}

.description {
  color: rgb(0 51 102 / 70%);
  font-size: clamp(16px, 2.1vw, 20px);
  line-height: 1.4;
  margin: 8px 0 0;
}

.action-row {
  align-items: flex-start;
  display: flex;
  gap: 24px;
  justify-content: space-between;
}

.input-box {
  border: 2px solid var(--navy);
  flex: 1;
  height: 169px;
  max-width: 990px;
  position: relative;
}

.placeholder {
  color: var(--navy);
  font-size: 16px;
  left: 24px;
  margin: 0;
  position: absolute;
  top: 20px;
}

.input-icon {
  height: 16px;
  left: 26px;
  position: absolute;
  top: 135px;
  width: 16px;
}

.input-icon svg,
.cta-icon {
  display: block;
  height: 100%;
  width: 100%;
}

.cta-button {
  align-items: center;
  background: var(--orange);
  border: 0;
  color: var(--cream);
  cursor: pointer;
  display: inline-flex;
  gap: 8px;
  height: 51.2px;
  justify-content: center;
  min-width: 170.262px;
  padding: 0 16px;
  white-space: nowrap;
}

.cta-button span {
  font-size: 16px;
  font-weight: 700;
  line-height: 1.4;
}

.cta-icon {
  flex: 0 0 20px;
  height: 20px;
  width: 20px;
}

.cube-illustration {
  height: 160px;
  pointer-events: none;
  position: absolute;
  right: 0;
  top: 10px;
  width: 233px;
  z-index: 1;
}

.cube {
  position: absolute;
}

.cube-1 {
  background: var(--orange);
  box-shadow: 4px 4px 0 0 var(--butter);
  height: 31.898px;
  left: 87.06px;
  opacity: 0.6;
  top: 23.36px;
  width: 31.898px;
  animation: cube1 3s ease-in-out infinite;
}

.cube-2 {
  background: var(--navy);
  box-shadow: 12px 12px 0 0 rgb(255 131 97 / 40%);
  height: 65.277px;
  left: 124.39px;
  top: 55.72px;
  width: 65.277px;
  animation: cube2 4s ease-in-out infinite;
}

.cube-3 {
  background: var(--butter);
  box-shadow: 6px 6px 0 0 rgb(0 51 102 / 30%);
  height: 45.171px;
  left: 160.04px;
  top: 94.85px;
  width: 45.171px;
  animation: cube3 3.5s ease-in-out infinite;
}

.cube-4 {
  background: #dedede;
  box-shadow: 5px 5px 0 0 rgb(0 51 102 / 20%);
  height: 34.129px;
  left: 196.08px;
  top: 0;
  width: 34.129px;
  animation: cube4 3.2s ease-in-out infinite;
}

.cube-5 {
  background: var(--orange);
  box-shadow: 4px 4px 0 0 rgb(0 51 102 / 20%);
  height: 31.898px;
  left: 35.38px;
  opacity: 0.6;
  top: 117.82px;
  width: 31.898px;
  animation: cube5 3.8s ease-in-out infinite;
}

.cube-6 {
  background: var(--orange);
  box-shadow: 8px 8px 0 0 rgb(0 51 102 / 30%);
  height: 50.227px;
  left: 0;
  top: 80px;
  width: 50.227px;
  animation: cube6 3.6s ease-in-out infinite;
}

@keyframes cube1 {
  0%,
  100% {
    opacity: 0.6;
    transform: translateY(0) scale(1) rotate(-60deg);
  }

  50% {
    opacity: 0.7;
    transform: translateY(-8px) scale(1.05) rotate(-55deg);
  }
}

@keyframes cube2 {
  0%,
  100% {
    opacity: 1;
    transform: translateY(0) scale(1) rotate(-2.02deg);
  }

  50% {
    opacity: 0.9;
    transform: translateY(-10px) scale(1.03) rotate(2deg);
  }
}

@keyframes cube3 {
  0%,
  100% {
    opacity: 1;
    transform: translateY(0) scale(1) rotate(9.09deg);
  }

  50% {
    opacity: 0.85;
    transform: translateY(-9px) scale(1.04) rotate(12deg);
  }
}

@keyframes cube4 {
  0%,
  100% {
    opacity: 1;
    transform: translateY(0) scale(1) rotate(-4.9deg);
  }

  50% {
    opacity: 0.9;
    transform: translateY(-7px) scale(1.05) rotate(-1deg);
  }
}

@keyframes cube5 {
  0%,
  100% {
    opacity: 0.6;
    transform: translateY(0) scale(1) rotate(9.8deg);
  }

  50% {
    opacity: 0.7;
    transform: translateY(-8px) scale(1.05) rotate(13deg);
  }
}

@keyframes cube6 {
  0%,
  100% {
    opacity: 1;
    transform: translateY(0) scale(1) rotate(3.64deg);
  }

  50% {
    opacity: 0.9;
    transform: translateY(-11px) scale(1.04) rotate(0deg);
  }
}

</style>
