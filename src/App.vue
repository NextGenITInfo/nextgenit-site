<template>
  <div class="container">
    <div class="content">
      <div class="logo-placeholder">
        <div class="logo-icon">NGIT</div>
      </div>
      <h1 class="title">NextGenIT</h1>
      <p class="description">
        Building the future of technology, one innovation at a time.
      </p>
      <div class="social-icons">
        <!-- Social icons placeholder for future implementation -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App'
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
  /* Prepared for animated background */
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}

.content {
  text-align: center;
  z-index: 1;
  max-width: 600px;
  animation: fadeIn 1s ease-in;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.logo-placeholder {
  margin-bottom: 2rem;
  display: flex;
  justify-content: center;
}

.logo-icon {
  width: 120px;
  height: 120px;
  background: rgba(255, 255, 255, 0.95);
  border-radius: 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 2rem;
  font-weight: 700;
  color: #667eea;
  box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
  transition: transform 0.3s ease;
}

.logo-icon:hover {
  transform: scale(1.05);
}

.title {
  font-size: 3rem;
  font-weight: 700;
  margin: 0 0 1rem 0;
  color: white;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
}

.description {
  font-size: 1.25rem;
  color: rgba(255, 255, 255, 0.95);
  line-height: 1.6;
  margin: 0;
}

.social-icons {
  margin-top: 2rem;
  /* Prepared for social icons */
}

/* Responsive design */
@media (max-width: 768px) {
  .title {
    font-size: 2rem;
  }
  
  .description {
    font-size: 1rem;
  }
  
  .logo-icon {
    width: 100px;
    height: 100px;
    font-size: 1.5rem;
  }
}

@media (max-width: 480px) {
  .title {
    font-size: 1.5rem;
  }
  
  .logo-icon {
    width: 80px;
    height: 80px;
    font-size: 1.25rem;
  }
}
</style>
