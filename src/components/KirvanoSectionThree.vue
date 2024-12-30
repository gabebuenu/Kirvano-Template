<template>
    <section class="premium-section">
      <div class="container">
        <div class="premium-header">
          <h2>Área de Membros Premium</h2>
          <p>
            Ofereça uma experiência verdadeiramente exclusiva e atraente através das
            nossas ferramentas de personalização.
          </p>
        </div>
  
        <div class="features-grid">
          <!-- Community Feature -->
          <div class="feature-card community">
            <div class="feature-content">
              <div class="feature-text">
                <h3>Conteúdo e comunidade juntos</h3>
                <p>
                  Engaje, dê suporte e crie conexão com o seu público através de uma
                  comunidade integrada.
                </p>
                <a href="#" class="feature-link">
                  Entrar agora
                  <ArrowRight class="icon" size="16" />
                </a>
              </div>
              <div class="feature-image community-image">
                <!-- <img src="/placeholder.svg?height=300&width=400" alt="Community interface" /> -->
              </div>
            </div>
          </div>
  
          <!-- Subscription Feature -->
          <div class="feature-card dark subscription">
            <div class="feature-content">
              <div class="feature-text">
                <h3>Crie assinaturas para conteúdos exclusivos</h3>
              </div>
              <div class="feature-image subscription-image">
                <!-- <img src="/placeholder.svg?height=300&width=400" alt="Subscription interface" /> -->
              </div>
            </div>
          </div>
  
          <!-- Analytics Feature -->
          <div class="feature-card dark analytics">
            <div class="feature-content">
              <div class="feature-text">
                <h3>Gestão ativa com dados e inteligência</h3>
              </div>
              <div class="feature-image analytics-image">
                <!-- <img src="/placeholder.svg?height=300&width=400" alt="Analytics graph" /> -->
              </div>
            </div>
          </div>
  
          <!-- Customization Feature -->
          <div class="feature-card dark customize">
            <div class="feature-content">
              <div class="feature-text">
                <h3>Customize com o que você precisa</h3>
              </div>
              <div class="toggle-list">
                <div class="toggle-item">
                  <span>Avaliações</span>
                  <div class="toggle active">
                    <div class="toggle-slider"></div>
                  </div>
                </div>
                <div class="toggle-item">
                  <span>Conteúdo</span>
                  <div class="toggle active">
                    <div class="toggle-slider"></div>
                  </div>
                </div>
                <div class="toggle-item">
                  <span>Clube de benefícios</span>
                  <div class="toggle active">
                    <div class="toggle-slider"></div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  import { ArrowRight } from 'lucide-vue-next'
  </script>
  
  <style>
  .premium-section {
    padding: 120px 0;
    background: #FFFFFF;
  }
  
  .container {
    max-width: 1240px;
    margin: 0 auto;
    padding: 0 24px;
  }
  
  .premium-header {
    text-align: center;
    max-width: 720px;
    margin: 0 auto 64px;
  }
  
  .premium-header h2 {
    font-size: 48px;
    font-weight: 800;
    line-height: 1.1;
    letter-spacing: -0.02em;
    margin-bottom: 24px;
    color: #000000;
  }
  
  .premium-header p {
    font-size: 20px;
    line-height: 1.5;
    color: #666666;
    padding: 0 24px;
  }
  
  .features-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 24px;
  }
  
  .feature-card {
    border-radius: 16px;
    overflow: hidden;
    position: relative;
    height: 360px;
  }
  
  .feature-card.community {
    background: #FFFFFF;
    border: 1px solid #EAEAEA;
  }
  
  .feature-card.dark {
    background: #1A1A1A;
    color: #FFFFFF;
  }
  
  .feature-content {
    height: 100%;
    padding: 40px;
    position: relative;
    z-index: 2;
  }
  
  .feature-text {
    max-width: 320px;
  }
  
  .feature-card h3 {
    font-size: 28px;
    font-weight: 700;
    line-height: 1.2;
    margin-bottom: 16px;
  }
  
  .feature-card.community p {
    font-size: 16px;
    line-height: 1.5;
    color: #666666;
    margin-bottom: 24px;
  }
  
  .feature-link {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    color: #0066FF;
    text-decoration: none;
    font-weight: 500;
    font-size: 16px;
  }
  
  .feature-image {
    position: absolute;
    z-index: 1;
  }
  
  .community-image {
    right: -5%;
    bottom: -5%;
    width: 65%;
  }
  
  .subscription-image {
    right: -5%;
    bottom: -5%;
    width: 50%;
  }
  
  .analytics-image {
    right: 0;
    bottom: 0;
    width: 100%;
    height: 100%;
    opacity: 0.9;
  }
  
  .toggle-list {
    position: absolute;
    right: 40px;
    top: 50%;
    transform: translateY(-50%);
    display: flex;
    flex-direction: column;
    gap: 16px;
  }
  
  .toggle-item {
    display: flex;
    align-items: center;
    gap: 12px;
    background: rgba(255, 255, 255, 0.1);
    padding: 8px 12px;
    border-radius: 8px;
  }
  
  .toggle-item span {
    font-size: 14px;
    font-weight: 500;
    color: #FFFFFF;
  }
  
  .toggle {
    width: 36px;
    height: 20px;
    background: rgba(255, 255, 255, 0.2);
    border-radius: 10px;
    position: relative;
    cursor: pointer;
  }
  
  .toggle.active {
    background: #0066FF;
  }
  
  .toggle-slider {
    width: 16px;
    height: 16px;
    background: #FFFFFF;
    border-radius: 50%;
    position: absolute;
    top: 2px;
    left: 2px;
    transition: transform 0.2s;
  }
  
  .toggle.active .toggle-slider {
    transform: translateX(16px);
  }
  
  @media (max-width: 1024px) {
    .premium-header h2 {
      font-size: 40px;
    }
  
    .feature-card {
      height: 320px;
    }
  
    .feature-card h3 {
      font-size: 24px;
    }
  }
  
  @media (max-width: 768px) {
    .features-grid {
      grid-template-columns: 1fr;
    }
  
    .feature-card {
      height: 280px;
    }
  
    .toggle-list {
      position: relative;
      right: auto;
      top: auto;
      transform: none;
      margin-top: 24px;
    }
  }
  
  @media (max-width: 640px) {
    .premium-header h2 {
      font-size: 32px;
      padding: 0 16px;
    }
  
    .premium-header p {
      font-size: 18px;
      padding: 0 16px;
    }
  
    .feature-content {
      padding: 24px;
    }
  
    .feature-text {
      max-width: 100%;
    }
  }
  </style>