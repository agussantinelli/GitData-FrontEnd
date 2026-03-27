<script setup lang="ts">
// GitData - Launch Page 
</script>

<template>
  <div class="landing-container">
    <div class="bg-glow"></div>
    
    <nav class="navbar">
      <div class="logo">
        <span class="gold-text">GIT</span>DATA.
      </div>
      <div class="nav-links">
        <a href="#about">Proyecto</a>
        <a href="#features">Motor</a>
        <button class="btn-outline">Ingresar</button>
      </div>
    </nav>

    <main class="hero">
      <div class="hero-content">
        <div class="badge">Motor de Ficha Técnica</div>
        <h1 class="hero-title">
          La <span class="gold-text">Identidad</span> <br/>
          de tu Código.
        </h1>
        <p class="hero-description">
          GitData transforma el ruido de tu GitHub en una narrativa técnica curada. 
          Descubre tu ADN técnico y destaca las joyas ocultas de tu carrera profesional.
        </p>
        
        <div class="action-group">
          <button class="btn-primary">Analizar Perfil</button>
          <button class="btn-secondary">Explorar Radar</button>
        </div>
      </div>

      <div class="hero-visual">
        <div class="radar-circle">
          <div class="radar-dot"></div>
          <div class="radar-line"></div>
        </div>
      </div>
    </main>

    <section id="features" class="features-grid">
      <div class="feature-card">
        <div class="feature-icon">🧬</div>
        <h3>Radar de ADN</h3>
        <p>Visualización dinámica del balance de tu especialización técnica (FE vs BE).</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon">💎</div>
        <h3>Joyas Ocultas</h3>
        <p>Identificación de proyectos de alta utilidad más allá de las estrellas y los forks.</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon">📜</div>
        <h3>Timeline Narrativa</h3>
        <p>Evolución cronológica de tus hitos técnicos y crecimiento de stack a través del tiempo.</p>
      </div>
    </section>

    <footer class="footer">
      <p>&copy; 2026 GitData // Construido para la comunidad de desarrolladores de élite.</p>
    </footer>
  </div>
</template>

<style scoped>
.landing-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2rem;
  overflow-x: hidden;
}

.bg-glow {
  position: fixed;
  top: -10%;
  right: -10%;
  width: 50vw;
  height: 50vw;
  background: radial-gradient(circle, rgba(0, 31, 63, 0.3) 0%, rgba(5, 5, 5, 0) 70%);
  z-index: -1;
  pointer-events: none;
}

.navbar {
  height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.5rem;
  font-weight: 800;
  letter-spacing: 3px;
}

.nav-links {
  display: flex;
  gap: 2rem;
  align-items: center;
}

.hero {
  display: grid;
  grid-template-columns: 1.2fr 0.8fr;
  gap: 4rem;
  align-items: center;
  min-height: 80vh;
}

.badge {
  display: inline-block;
  padding: 0.5rem 1rem;
  background: rgba(0, 31, 63, 0.5);
  border: 1px solid var(--gold);
  border-radius: 50px;
  font-size: 0.8rem;
  text-transform: uppercase;
  color: var(--gold);
  margin-bottom: 2rem;
}

.hero-title {
  font-size: 5rem;
  line-height: 1;
  margin-bottom: 2rem;
}

.hero-description {
  font-size: 1.2rem;
  color: var(--silver);
  max-width: 600px;
  margin-bottom: 3rem;
  opacity: 0.8;
}

.action-group {
  display: flex;
  gap: 1.5rem;
}

.btn-primary {
  background: var(--gold);
  color: var(--black);
  padding: 1rem 2rem;
  border: none;
  font-weight: 700;
  text-transform: uppercase;
  cursor: pointer;
  border-radius: 4px;
}

.btn-secondary {
  background: transparent;
  color: var(--white);
  padding: 1rem 2rem;
  border: 1px solid rgba(255, 255, 255, 0.2);
  font-weight: 700;
  text-transform: uppercase;
  cursor: pointer;
  border-radius: 4px;
}

.btn-outline {
  background: transparent;
  color: var(--gold);
  padding: 0.5rem 1.5rem;
  border: 1px solid var(--gold);
  border-radius: 4px;
  cursor: pointer;
}

.hero-visual {
  display: flex;
  justify-content: center;
}

.radar-circle {
  width: 300px;
  height: 300px;
  border: 1px solid rgba(175, 149, 0, 0.2);
  border-radius: 50%;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
}

.radar-circle::before {
  content: '';
  width: 200px;
  height: 200px;
  border: 1px solid rgba(175, 149, 0, 0.1);
  border-radius: 50%;
  position: absolute;
}

.radar-line {
  width: 50%;
  height: 1px;
  background: linear-gradient(90deg, rgba(175, 149, 0, 0.5) 0%, transparent 100%);
  position: absolute;
  top: 50%;
  left: 0;
  transform-origin: right center;
  animation: rotate 4s linear infinite;
}

@keyframes rotate {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

.features-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2rem;
  padding: 6rem 0;
  border-top: 1px solid rgba(255, 255, 255, 0.05);
}

.feature-card {
  padding: 2.5rem;
  background: rgba(255, 255, 255, 0.02);
  border: 1px solid rgba(255, 255, 255, 0.05);
  border-radius: 12px;
  transition: transform 0.3s;
}

.feature-card:hover {
  transform: translateY(-10px);
  border-color: var(--gold);
}

.feature-icon {
  font-size: 2.5rem;
  margin-bottom: 1.5rem;
}

.feature-card h3 {
  margin-bottom: 1rem;
}

.footer {
  padding: 4rem 0;
  text-align: center;
  border-top: 1px solid rgba(255, 255, 255, 0.05);
  font-size: 0.9rem;
  opacity: 0.5;
}

@media (max-width: 1024px) {
  .hero {
    grid-template-columns: 1fr;
    text-align: center;
    padding-top: 4rem;
  }
  .hero-title { font-size: 3.5rem; }
  .features-grid { grid-template-columns: 1fr; }
  .action-group { justify-content: center; }
  .nav-links a { display: none; }
}
</style>
