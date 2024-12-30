<template>
    <div class="landing-page">
      <!-- Top Banner -->
      <div class="top-banner">
        <div class="container">
          <div class="banner-content">
            <span class="banner-dot">●</span>
            <p>Fatura acima de 100 mil? Tenha um gerente de contas exclusivo.</p>
            <button class="banner-button">
              <PhoneCall class="icon" size="14" />
              Falar com especialista
            </button>
          </div>
        </div>
      </div>
  
      <!-- Navigation -->
      <nav class="navbar">
        <div class="container nav-container">
          <a href="/" class="logo">kirvano</a>
          <div class="nav-links">
            <a href="#" class="nav-link">Início</a>
            <a href="#" class="nav-link">Funcionalidades</a>
            <a href="#" class="nav-link">Planos e taxas</a>
            <a href="#" class="nav-link">Ajuda</a>
          </div>
          <div class="auth-buttons">
            <a href="#" class="login">Login</a>
            <a href="#" class="signup">Cadastre-se agora</a>
          </div>
        </div>
      </nav>
  
      <!-- Hero Section -->
      <section class="hero">
        <div class="container hero-container">
          <div class="hero-content">
            <h1>
              Simples,
              <br />
              confiável, lucrativa,
              <br />
              para pessoas ambiciosas
            </h1>
            <p>
              Crie produtos e serviços digitais como e-books, cursos online,
              mentorias — e venda com a menor taxa do mercado.
            </p>
            <button class="cta-button">
              Cadastre-se agora
              <ArrowRight class="icon" size="20" />
            </button>
          </div>
          <div class="hero-image">
            <!-- <img src="/placeholder.svg?height=600&width=600" alt="Plataforma de pagamentos online" /> -->
          </div>
        </div>
      </section>
    </div>
  </template>
  
  <script setup>
  import { PhoneCall, ArrowRight } from 'lucide-vue-next'
  </script>
  
  <style>
  /* Reset and Base Styles */
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
    -webkit-font-smoothing: antialiased;
    line-height: 1.5;
  }
  
  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 24px;
  }
  
  /* Top Banner */
  .top-banner {
    background: #1A1A1A;
    padding: 8px 0;
  }
  
  .banner-content {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 8px;
  }
  
  .banner-content p {
    color: #FFFFFF;
    font-size: 14px;
    font-weight: 400;
  }
  
  .banner-dot {
    color: #0066FF;
    font-size: 8px;
  }
  
  .banner-button {
    display: flex;
    align-items: center;
    gap: 6px;
    background: #FFFFFF;
    border: none;
    border-radius: 16px;
    padding: 4px 12px;
    font-size: 14px;
    cursor: pointer;
  }
  
  .banner-button .icon {
    color: #000000;
  }
  
  /* Navigation */
  .navbar {
    padding: 24px 0;
    border-bottom: 1px solid #EAEAEA;
  }
  
  .nav-container {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  
  .logo {
    color: #000000;
    font-size: 24px;
    font-weight: 700;
    text-decoration: none;
    letter-spacing: -0.5px;
  }
  
  .nav-links {
    display: flex;
    gap: 40px;
  }
  
  .nav-link {
    color: #000000;
    text-decoration: none;
    font-size: 15px;
    font-weight: 500;
  }
  
  .auth-buttons {
    display: flex;
    align-items: center;
    gap: 24px;
  }
  
  .login {
    color: #0066FF;
    text-decoration: none;
    font-weight: 500;
  }
  
  .signup {
    background: #0066FF;
    color: #FFFFFF;
    text-decoration: none;
    padding: 12px 24px;
    border-radius: 4px;
    font-weight: 500;
  }
  
  /* Hero Section */
  .hero {
    padding: 64px 0;
  }
  
  .hero-container {
    display: grid;
    grid-template-columns: minmax(0, 1fr) minmax(0, 1fr);
    gap: 64px;
    align-items: center;
  }
  
  .hero-content h1 {
    font-size: 56px;
    line-height: 1.1;
    font-weight: 800;
    letter-spacing: -0.02em;
    margin-bottom: 24px;
    color: #000000;
  }
  
  .hero-content p {
    font-size: 20px;
    line-height: 1.5;
    color: #666666;
    margin-bottom: 32px;
    max-width: 520px;
  }
  
  .cta-button {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    background: #0066FF;
    color: #FFFFFF;
    border: none;
    padding: 16px 32px;
    border-radius: 4px;
    font-size: 16px;
    font-weight: 500;
    cursor: pointer;
  }
  
  .hero-image {
    position: relative;
  }
  
  .hero-image img {
    width: 100%;
    height: auto;
  }
  
  /* Responsive Design */
  @media (max-width: 768px) {
    .nav-links {
      display: none;
    }
  
    .hero-container {
      grid-template-columns: 1fr;
      text-align: center;
    }
  
    .hero-content p {
      margin-left: auto;
      margin-right: auto;
    }
  
    .auth-buttons {
      display: none;
    }
  }
  
  @media (max-width: 640px) {
    .banner-content {
      flex-direction: column;
      gap: 8px;
    }
  
    .hero-content h1 {
      font-size: 40px;
    }
  
    .hero-content p {
      font-size: 18px;
    }
  }
  </style>