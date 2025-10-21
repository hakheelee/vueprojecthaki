<template>
  <div class="app-container">
    <header class="app-header">
      <h1>🎵 Duckin Music</h1>
      <p class="tagline">Your Ultimate Music Experience</p>
    </header>
    
    <main class="app-main">
      <section class="hero-section">
        <div class="music-icon">🎧</div>
        <h2>Welcome to Duckin Music</h2>
        <p>Discover, stream, and enjoy your favorite tracks</p>
      </section>
      
      <section class="features">
        <div class="feature-card">
          <div class="feature-icon">🎸</div>
          <h3>Browse Music</h3>
          <p>Explore millions of songs</p>
        </div>
        
        <div class="feature-card">
          <div class="feature-icon">📻</div>
          <h3>Radio Stations</h3>
          <p>Listen to live radio</p>
        </div>
        
        <div class="feature-card">
          <div class="feature-icon">💿</div>
          <h3>Playlists</h3>
          <p>Create your own vibe</p>
        </div>
      </section>
      
      <button class="cta-button">Get Started</button>
    </main>
    
    <footer class="app-footer">
      <p>iPhone 15 Pro Optimized (391 x 857)</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style scoped>
.app-container {
  width: 100%;
  height: 100%;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  display: flex;
  flex-direction: column;
  overflow-y: auto;
}

.app-header {
  padding: 20px;
  text-align: center;
  background: rgba(0, 0, 0, 0.2);
  backdrop-filter: blur(10px);
}

.app-header h1 {
  font-size: 28px;
  margin-bottom: 8px;
  font-weight: 700;
}

.tagline {
  font-size: 14px;
  opacity: 0.9;
}

.app-main {
  flex: 1;
  padding: 20px;
  display: flex;
  flex-direction: column;
  gap: 24px;
  overflow-y: auto;
}

.hero-section {
  text-align: center;
  padding: 30px 0;
}

.music-icon {
  font-size: 80px;
  margin-bottom: 20px;
  animation: pulse 2s ease-in-out infinite;
}

@keyframes pulse {
  0%, 100% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.1);
  }
}

.hero-section h2 {
  font-size: 24px;
  margin-bottom: 12px;
}

.hero-section p {
  font-size: 16px;
  opacity: 0.9;
}

.features {
  display: flex;
  flex-direction: column;
  gap: 16px;
}

.feature-card {
  background: rgba(255, 255, 255, 0.15);
  backdrop-filter: blur(10px);
  border-radius: 16px;
  padding: 20px;
  text-align: center;
  transition: transform 0.2s, box-shadow 0.2s;
}

.feature-card:active {
  transform: scale(0.98);
}

.feature-icon {
  font-size: 40px;
  margin-bottom: 12px;
}

.feature-card h3 {
  font-size: 18px;
  margin-bottom: 8px;
}

.feature-card p {
  font-size: 14px;
  opacity: 0.9;
}

.cta-button {
  background: white;
  color: #667eea;
  border: none;
  border-radius: 25px;
  padding: 16px 32px;
  font-size: 18px;
  font-weight: 600;
  cursor: pointer;
  transition: transform 0.2s, box-shadow 0.2s;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.2);
}

.cta-button:active {
  transform: scale(0.98);
}

.app-footer {
  padding: 16px;
  text-align: center;
  font-size: 12px;
  background: rgba(0, 0, 0, 0.2);
  opacity: 0.8;
}
</style>
