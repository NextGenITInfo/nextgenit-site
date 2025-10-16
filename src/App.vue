<template>
  <div class="container">
    <!-- Animated cosmic background -->
    <div class="animated-bg">
      <!-- Distant stars -->
      <div class="stars-layer">
        <span v-for="s in 80" :key="s" class="star" :style="getStarStyle(s)"></span>
      </div>
      
      <!-- Geometric planets -->
      <div class="planets">
        <div v-for="p in 4" :key="p" class="planet" :style="getPlanetStyle(p)"></div>
      </div>
      
      <!-- Floating geometric shapes -->
      <div class="geometric-shapes">
        <div v-for="g in 6" :key="g" class="geometric-shape" :style="getGeometricStyle(g)"></div>
      </div>
      
      <!-- Cosmic grid lines -->
      <div class="cosmic-grid"></div>
      
      <!-- Nebula clouds -->
      <div class="nebula" v-for="n in 3" :key="n" :style="getNebulaStyle(n)"></div>
      
      <!-- Subtle floating particles -->
      <div class="particles">
        <div v-for="p in 12" :key="p" class="particle" :style="getParticleStyle(p)"></div>
      </div>
      
      <!-- Elegant gradient overlays -->
      <div class="gradient-overlay"></div>
    </div>

    <div class="content">
      <div class="logo-placeholder">
        <img class="logo-img" src="/src/assets/NextGenIT_logo_transparent.png" alt="NextGenIT" />
      </div>
      <h1 class="title">NextGenIT</h1>
      <p class="description">
        NextGenIT to cykl spotkań, który inspiruje młode pokolenie do odkrywania, tworzenia i rozwoju w świecie nowych technologii. Łączymy przyszłych i obecnych specjalistów IT, tworząc przestrzeń wymiany wiedzy, doświadczeń i inspiracji.
      </p>
      <div class="quizzes">
        <div class="quiz-card">
          <div class="quiz-info">
            <h2 class="quiz-title">Quiz 1</h2>
            <p class="quiz-time">Start: 10:00 • Koniec: 13:30 • Wręczenie nagród: 13:50</p>
          </div>
          <a class="quiz-btn" href="https://docs.google.com/forms/d/e/1FAIpQLSeu_SybcchIAd5lyg4WVwy0LGMCMe_sA4_R1OtVk3MmlXr2IA/viewform?usp=dialog" target="_blank" rel="noopener noreferrer">Weź udział</a>
        </div>
        <div class="quiz-card">
          <div class="quiz-info">
            <h2 class="quiz-title">Quiz 2</h2>
            <p class="quiz-time">Start: 14:00 • Koniec: 15:30 • Wręczenie nagród: 15:50</p>
          </div>
          <a class="quiz-btn" href="https://docs.google.com/forms/d/e/1FAIpQLSekfGxdxWy2qDPpVjg9B9Xiuritb-974z9UGq4y46w622UNXg/viewform?usp=dial" target="_blank" rel="noopener noreferrer">Weź udział</a>
        </div>
      </div>
      <p class="follow-label">Zachęcamy do obserwowania!</p>
      <div class="social-icons">
        <a href="https://www.facebook.com/nextgenitkrk" target="_blank" rel="noopener noreferrer" class="social-link">
          <svg class="social-icon" viewBox="0 0 24 24" fill="currentColor">
            <path d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"/>
          </svg>
        </a>
        <a href="https://www.instagram.com/nextgenit.krk/" target="_blank" rel="noopener noreferrer" class="social-link">
          <svg class="social-icon" viewBox="0 0 24 24" fill="currentColor">
            <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/>
          </svg>
        </a>
        <a href="https://www.linkedin.com/company/nextgenit-krakow/" target="_blank" rel="noopener noreferrer" class="social-link">
          <svg class="social-icon" viewBox="0 0 24 24" fill="currentColor">
            <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>
          </svg>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  methods: {
    getStarStyle(index) {
      const size = Math.random() * 3 + 1; // 1-4px
      const left = Math.random() * 100;
      const top = Math.random() * 100;
      const delay = Math.random() * 8;
      const brightness = Math.random() * 0.5 + 0.5; // 0.5-1.0
      return {
        width: `${size}px`,
        height: `${size}px`,
        left: `${left}%`,
        top: `${top}%`,
        animationDelay: `${delay}s`,
        opacity: brightness
      };
    },
    getPlanetStyle(index) {
      const sizes = [120, 80, 60, 40];
      const size = sizes[index % sizes.length];
      const left = Math.random() * 80 + 10; // 10-90%
      const top = Math.random() * 60 + 20; // 20-80%
      const duration = Math.random() * 30 + 20; // 20-50s
      const delay = Math.random() * -30;
      const rotation = Math.random() * 360;
      return {
        width: `${size}px`,
        height: `${size}px`,
        left: `${left}%`,
        top: `${top}%`,
        animationDuration: `${duration}s`,
        animationDelay: `${delay}s`,
        transform: `rotate(${rotation}deg)`
      };
    },
    getGeometricStyle(index) {
      const shapes = ['triangle', 'square', 'hexagon', 'diamond'];
      const shape = shapes[index % shapes.length];
      const size = Math.random() * 40 + 20; // 20-60px
      const left = Math.random() * 100;
      const top = Math.random() * 100;
      const duration = Math.random() * 25 + 15; // 15-40s
      const delay = Math.random() * -25;
      const rotation = Math.random() * 360;
      return {
        width: `${size}px`,
        height: `${size}px`,
        left: `${left}%`,
        top: `${top}%`,
        animationDuration: `${duration}s`,
        animationDelay: `${delay}s`,
        transform: `rotate(${rotation}deg)`,
        '--shape-type': shape
      };
    },
    getNebulaStyle(index) {
      const size = Math.random() * 300 + 200; // 200-500px
      const left = Math.random() * 100;
      const top = Math.random() * 100;
      const duration = Math.random() * 40 + 30; // 30-70s
      const delay = Math.random() * -40;
      const opacity = Math.random() * 0.3 + 0.1; // 0.1-0.4
      return {
        width: `${size}px`,
        height: `${size}px`,
        left: `${left}%`,
        top: `${top}%`,
        animationDuration: `${duration}s`,
        animationDelay: `${delay}s`,
        opacity: opacity
      };
    },
    getParticleStyle(index) {
      const size = Math.random() * 3 + 1; // 1-4px
      const left = Math.random() * 100;
      const top = Math.random() * 100;
      const duration = Math.random() * 15 + 10; // 10-25s
      const delay = Math.random() * -15;
      const opacity = Math.random() * 0.4 + 0.2; // 0.2-0.6
      return {
        width: `${size}px`,
        height: `${size}px`,
        left: `${left}%`,
        top: `${top}%`,
        animationDuration: `${duration}s`,
        animationDelay: `${delay}s`,
        opacity: opacity
      };
    }
  }
}
</script>

<style scoped>
.container {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 2rem;
  position: relative;
  overflow: hidden;
  background: var(--primary-gradient);
}

/* Cosmic background elements */
.animated-bg {
  position: fixed;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  z-index: 0;
  overflow: hidden;
  background: radial-gradient(ellipse at center, #18204E 0%, #0F1A3A 50%, #0A1220 100%);
}

.stars-layer {
  position: absolute;
  inset: 0;
  pointer-events: none;
}

.star {
  position: absolute;
  display: block;
  background: rgba(201, 255, 255, 0.7);
  border-radius: 50%;
  box-shadow: 
    0 0 4px rgba(201, 255, 255, 0.6),
    0 0 8px rgba(0, 255, 209, 0.2);
  animation: starTwinkle 6s ease-in-out infinite;
}

.planets {
  position: absolute;
  inset: 0;
  pointer-events: none;
}

.planet {
  position: absolute;
  border-radius: 50%;
  background: radial-gradient(circle at 30% 30%, 
    rgba(0, 255, 209, 0.2), 
    rgba(254, 0, 91, 0.15), 
    rgba(24, 32, 78, 0.8));
  box-shadow: 
    inset -15px -15px 30px rgba(0, 0, 0, 0.4),
    0 0 12px rgba(0, 255, 209, 0.1);
  animation: planetOrbit linear infinite;
}

.geometric-shapes {
  position: absolute;
  inset: 0;
  pointer-events: none;
}

.geometric-shape {
  position: absolute;
  background: linear-gradient(45deg, 
    rgba(0, 255, 209, 0.15), 
    rgba(254, 0, 91, 0.1));
  border: 1px solid rgba(201, 255, 255, 0.3);
  animation: geometricFloat linear infinite;
}

.geometric-shape::before {
  content: '';
  position: absolute;
  inset: 0;
  background: inherit;
  border: inherit;
  transform: rotate(45deg);
  opacity: 0.5;
}

.geometric-shape:nth-child(odd) {
  clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
}

.geometric-shape:nth-child(even) {
  clip-path: polygon(25% 0%, 75% 0%, 100% 50%, 75% 100%, 25% 100%, 0% 50%);
}

.cosmic-grid {
  position: absolute;
  inset: 0;
  background-image: 
    linear-gradient(rgba(201, 255, 255, 0.1) 1px, transparent 1px),
    linear-gradient(90deg, rgba(201, 255, 255, 0.1) 1px, transparent 1px);
  background-size: 50px 50px;
  animation: gridPulse 8s ease-in-out infinite;
  opacity: 0.3;
}

.nebula {
  position: absolute;
  background: radial-gradient(ellipse, 
    rgba(0, 255, 209, 0.1) 0%, 
    rgba(254, 0, 91, 0.08) 30%, 
    transparent 70%);
  border-radius: 50%;
  filter: blur(40px);
  animation: nebulaDrift linear infinite;
}

@keyframes starTwinkle {
  0%, 100% { 
    opacity: 0.4; 
    transform: scale(1); 
  }
  50% { 
    opacity: 1; 
    transform: scale(1.3); 
  }
}

@keyframes planetOrbit {
  0% { 
    transform: translate3d(0, 0, 0) rotate(0deg); 
    opacity: 0.6; 
  }
  25% { 
    transform: translate3d(20vw, -10vh, 0) rotate(90deg); 
    opacity: 0.8; 
  }
  50% { 
    transform: translate3d(-10vw, 20vh, 0) rotate(180deg); 
    opacity: 0.7; 
  }
  75% { 
    transform: translate3d(-20vw, -5vh, 0) rotate(270deg); 
    opacity: 0.9; 
  }
  100% { 
    transform: translate3d(0, 0, 0) rotate(360deg); 
    opacity: 0.6; 
  }
}

@keyframes geometricFloat {
  0% { 
    transform: translate3d(0, 0, 0) rotate(0deg); 
    opacity: 0.3; 
  }
  33% { 
    transform: translate3d(15vw, -15vh, 0) rotate(120deg); 
    opacity: 0.6; 
  }
  66% { 
    transform: translate3d(-10vw, 20vh, 0) rotate(240deg); 
    opacity: 0.4; 
  }
  100% { 
    transform: translate3d(0, 0, 0) rotate(360deg); 
    opacity: 0.3; 
  }
}

@keyframes gridPulse {
  0%, 100% { opacity: 0.2; }
  50% { opacity: 0.5; }
}

@keyframes nebulaDrift {
  0% { 
    transform: translate3d(-20vw, -10vh, 0) scale(0.8); 
    opacity: 0.1; 
  }
  25% { 
    transform: translate3d(10vw, -20vh, 0) scale(1.2); 
    opacity: 0.3; 
  }
  50% { 
    transform: translate3d(20vw, 10vh, 0) scale(0.9); 
    opacity: 0.2; 
  }
  75% { 
    transform: translate3d(-10vw, 20vh, 0) scale(1.1); 
    opacity: 0.4; 
  }
  100% { 
    transform: translate3d(-20vw, -10vh, 0) scale(0.8); 
    opacity: 0.1; 
  }
}

/* Subtle floating particles */
.particles {
  position: absolute;
  inset: 0;
  pointer-events: none;
}

.particle {
  position: absolute;
  background: rgba(201, 255, 255, 0.4);
  border-radius: 50%;
  animation: particleFloat linear infinite;
}

.gradient-overlay {
  position: absolute;
  inset: 0;
  background: 
    radial-gradient(ellipse at 20% 20%, rgba(0, 255, 209, 0.05) 0%, transparent 50%),
    radial-gradient(ellipse at 80% 80%, rgba(254, 0, 91, 0.03) 0%, transparent 50%),
    radial-gradient(ellipse at 50% 50%, rgba(24, 32, 78, 0.1) 0%, transparent 70%);
  animation: gradientShift 20s ease-in-out infinite;
}

@keyframes particleFloat {
  0% { 
    transform: translate3d(0, 0, 0) scale(0.8); 
    opacity: 0.3; 
  }
  25% { 
    transform: translate3d(10vw, -15vh, 0) scale(1.2); 
    opacity: 0.6; 
  }
  50% { 
    transform: translate3d(-5vw, 20vh, 0) scale(0.9); 
    opacity: 0.4; 
  }
  75% { 
    transform: translate3d(-15vw, -5vh, 0) scale(1.1); 
    opacity: 0.7; 
  }
  100% { 
    transform: translate3d(0, 0, 0) scale(0.8); 
    opacity: 0.3; 
  }
}

@keyframes gradientShift {
  0%, 100% { 
    opacity: 0.3; 
    transform: scale(1); 
  }
  50% { 
    opacity: 0.6; 
    transform: scale(1.1); 
  }
}

.content {
  text-align: center;
  z-index: 1;
  max-width: 900px;
  padding: 2.5rem 1.5rem;
  animation: fadeIn 1.2s ease-out;
  position: relative;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(30px) scale(0.95);
  }
  to {
    opacity: 1;
    transform: translateY(0) scale(1);
  }
}

.logo-placeholder {
  margin-bottom: 1.75rem;
  display: flex;
  justify-content: center;
}

.logo-img {
  width: 220px;
  height: auto;
  filter: drop-shadow(0 4px 8px rgba(0, 0, 0, 0.3)) drop-shadow(0 0 16px rgba(0, 255, 209, 0.15));
  transition: all 0.3s ease;
}

.logo-img:hover {
  transform: scale(1.02);
  filter: drop-shadow(0 6px 12px rgba(0, 0, 0, 0.4)) drop-shadow(0 0 20px rgba(0, 255, 209, 0.25));
}

.title {
  font-size: 3.25rem;
  font-weight: 700;
  margin: 0 0 1.25rem 0;
  color: var(--text-primary);
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.3), 0 0 8px rgba(0, 255, 209, 0.2);
  animation: titleSubtle 4s ease-in-out infinite alternate;
  font-family: var(--font-title);
  position: relative;
}


@keyframes titleSubtle {
  from {
    text-shadow: 0 2px 4px rgba(0, 0, 0, 0.3), 0 0 8px rgba(0, 255, 209, 0.2);
  }
  to {
    text-shadow: 0 2px 4px rgba(0, 0, 0, 0.3), 0 0 12px rgba(0, 255, 209, 0.3);
  }
}


.description {
  font-size: 1.2rem;
  color: var(--text-secondary);
  line-height: 1.8;
  margin: 0 0 2.25rem 0;
  font-weight: 400;
  max-width: 820px;
  margin-left: auto;
  margin-right: auto;
  text-wrap: balance;
}

.social-icons {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin-top: 2rem;
}

.social-link {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 60px;
  height: 60px;
  background: rgba(24, 32, 78, 0.4);
  backdrop-filter: blur(8px);
  border: 1px solid rgba(201, 255, 255, 0.2);
  border-radius: 50%;
  color: var(--light-accent);
  text-decoration: none;
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
  position: relative;
  overflow: hidden;
}

.social-link::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(45deg, var(--primary), var(--secondary));
  opacity: 0;
  transition: opacity 0.3s ease;
  border-radius: 50%;
}

.social-link:hover::before {
  opacity: 0.2;
}

.social-link:hover {
  transform: translateY(-3px) scale(1.05);
  box-shadow: 
    0 8px 20px rgba(0, 0, 0, 0.3),
    0 0 12px rgba(0, 255, 209, 0.2);
  color: var(--primary);
  border-color: rgba(0, 255, 209, 0.4);
}

.social-icon {
  width: 28px;
  height: 28px;
  position: relative;
  z-index: 1;
  transition: all 0.3s ease;
}

.social-link:hover .social-icon {
  transform: scale(1.1);
}

/* Follow label */
.follow-label {
  color: var(--text-primary);
  font-family: var(--font-title);
  font-size: 1.5rem; /* slightly smaller than the 3.25rem title */
  font-weight: 700;
  letter-spacing: 0.3px;
  margin-top: 2.50rem;
  margin-bottom: 0.25rem;
}

/* Quizzes section */
.quizzes {
  display: grid;
  grid-template-columns: repeat(2, minmax(240px, 1fr));
  gap: 1rem;
  margin: 1.25rem auto 1.25rem auto; /* extra bottom space before follow label */
  max-width: 820px;
}

.quiz-card {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 1.25rem;
  border-radius: 14px;
  background: rgba(24, 32, 78, 0.45);
  border: 1px solid rgba(201, 255, 255, 0.18);
  backdrop-filter: blur(8px);
}

.quiz-info {
  text-align: left;
}

.quiz-title {
  margin: 0 0 0.25rem 0;
  font-family: var(--font-title);
  font-size: 1.25rem;
  color: var(--text-primary);
}

.quiz-time {
  margin: 0;
  font-size: 0.95rem;
  color: var(--text-secondary);
}

.quiz-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 0.55rem 1.1rem;
  border-radius: 10px;
  text-decoration: none;
  color: #0b1633;
  background: linear-gradient(135deg, var(--primary), #6dffe8);
  border: 1px solid rgba(0, 255, 209, 0.5);
  transition: transform 0.2s ease, box-shadow 0.2s ease, background 0.2s ease;
  font-family: var(--font-body);
  font-weight: 600;
  letter-spacing: 0.2px;
  line-height: 1; /* tighter */
  white-space: nowrap;
}

.quiz-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 24px rgba(0, 255, 209, 0.18);
  background: linear-gradient(135deg, #6dffe8, var(--primary));
}

@media (max-width: 768px) {
  .quizzes {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 640px) {
  .quiz-card {
    flex-direction: column;
    align-items: stretch;
    gap: 0.75rem;
  }
  .quiz-info {
    text-align: left;
  }
  .quiz-btn {
    width: 100%;
  }
}

/* Responsive design */
@media (max-width: 768px) {
  .content {
    padding: 2rem 1.25rem;
    max-width: 90%;
  }
  
  .title {
    font-size: 2.4rem;
  }
  
  .description {
    font-size: 1.1rem;
  }
  
  .logo-img {
    width: 180px;
  }
  
  .social-icons {
    gap: 1.5rem;
  }
  
  .social-link {
    width: 50px;
    height: 50px;
  }
  
  .social-icon {
    width: 24px;
    height: 24px;
  }
}

@media (max-width: 480px) {
  .container {
    padding: 1rem;
  }
  
  .content {
    padding: 1.5rem 1rem;
  }
  
  .title {
    font-size: 2rem;
  }
  
  .description {
    font-size: 1rem;
  }
  
  .logo-img {
    width: 140px;
  }
  
  .social-icons {
    gap: 1rem;
  }
  
  .social-link {
    width: 45px;
    height: 45px;
  }
  
  .social-icon {
    width: 20px;
    height: 20px;
  }
}

@media (max-width: 360px) {
  .logo-img {
    width: 120px;
  }
}
</style>
