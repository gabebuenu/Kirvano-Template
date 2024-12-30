<template>
    <div class="integrations-container">
      <!-- Integrations Section -->
      <section class="integrations">
        <div class="integrations-header">
          <h2>Integrações</h2>
          <p>Você pode contar com as principais integrações para que seu negócio tenha os melhores resultados.</p>
        </div>
  
        <div class="platforms">
          <div class="platforms-header">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
              <path d="M3 3h18v18H3z M8 12h8 M12 8v8"/>
            </svg>
            <span>Plataformas para realizar integrações</span>
          </div>
  
          <!-- Integration Partners Slider -->
          <div class="partners-slider">
            <div class="partners-track">
              <!-- <img src="/placeholder.svg?text=notzz" alt="Notzz" class="partner-logo" />
              <img src="/placeholder.svg?text=PayPIX" alt="PayPIX" class="partner-logo" />
              <img src="/placeholder.svg?text=Cademi" alt="Cademi" class="partner-logo" />
              <img src="/placeholder.svg?text=leadlovers" alt="Leadlovers" class="partner-logo" />
              <img src="/placeholder.svg?text=webhooks" alt="Webhooks" class="partner-logo" />
              <img src="/placeholder.svg?text=Plugo" alt="Plugo" class="partner-logo" />
              <img src="/placeholder.svg?text=memberkit" alt="Memberkit" class="partner-logo" />
              <img src="/placeholder.svg?text=mailchimp" alt="Mailchimp" class="partner-logo" />
              <img src="/placeholder.svg?text=hotmart" alt="Hotmart" class="partner-logo" />
              <img src="/placeholder.svg?text=voxcity" alt="Voxcity" class="partner-logo" /> -->
            </div>
            <!-- Duplicate track for infinite scroll effect -->
            <div class="partners-track">
              <!-- <img src="/placeholder.svg?text=notzz" alt="Notzz" class="partner-logo" />
              <img src="/placeholder.svg?text=PayPIX" alt="PayPIX" class="partner-logo" />
              <img src="/placeholder.svg?text=Cademi" alt="Cademi" class="partner-logo" />
              <img src="/placeholder.svg?text=leadlovers" alt="Leadlovers" class="partner-logo" />
              <img src="/placeholder.svg?text=webhooks" alt="Webhooks" class="partner-logo" />
              <img src="/placeholder.svg?text=Plugo" alt="Plugo" class="partner-logo" />
              <img src="/placeholder.svg?text=memberkit" alt="Memberkit" class="partner-logo" />
              <img src="/placeholder.svg?text=mailchimp" alt="Mailchimp" class="partner-logo" />
              <img src="/placeholder.svg?text=hotmart" alt="Hotmart" class="partner-logo" />
              <img src="/placeholder.svg?text=voxcity" alt="Voxcity" class="partner-logo" /> -->
            </div>
          </div>
  
          <!-- Webhooks Card -->
          <div class="integration-card">
            <div class="card-header">
              <!-- <img src="/placeholder.svg?text=webhooks" alt="Webhooks" class="card-logo" /> -->
              <button class="add-button">+</button>
            </div>
            <h3>Webhooks</h3>
            <p>Recurso que possibilita a comunicação entre duas ferramentas, fornecendo dados em tempo real.</p>
          </div>
        </div>
      </section>
  
      <!-- Blog Section -->
      <section class="blog-section">
        <div class="blog-content">
          <div class="blog-text">
            <h2>Mergulhe no universo da Kirvano</h2>
            <p>Visite nosso blog, sua nova fonte de conhecimento em tecnologia, negócios, boas práticas para vendas e muito mais.</p>
            <a href="#" class="blog-button">
              Acessar blog
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                <path d="M7 17l9.2-9.2M17 17V8h-9"/>
              </svg>
            </a>
          </div>
          <div class="ebooks-visual">
            <div class="ebook ebook-1"></div>
            <div class="ebook ebook-2"></div>
          </div>
        </div>
      </section>
    </div>
  </template>
  
  <style scoped>
  .integrations-container {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  }
  
  .integrations {
    padding: 80px 20px;
    max-width: 1200px;
    margin: 0 auto;
  }
  
  .integrations-header {
    text-align: center;
    margin-bottom: 60px;
  }
  
  .integrations-header h2 {
    font-size: 40px;
    font-weight: bold;
    margin-bottom: 16px;
  }
  
  .integrations-header p {
    color: #666;
    max-width: 600px;
    margin: 0 auto;
  }
  
  .platforms-header {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 40px;
    color: #666;
  }
  
  .partners-slider {
    position: relative;
    overflow: hidden;
    padding: 20px 0;
    margin-bottom: 40px;
  }
  
  .partners-track {
    display: flex;
    gap: 40px;
    animation: scroll 30s linear infinite;
  }
  
  @keyframes scroll {
    0% {
      transform: translateX(0);
    }
    100% {
      transform: translateX(-100%);
    }
  }
  
  .partner-logo {
    height: 40px;
    object-fit: contain;
  }
  
  .integration-card {
    background: white;
    border-radius: 12px;
    padding: 24px;
    border: 1px solid #eee;
    max-width: 400px;
  }
  
  .card-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 16px;
  }
  
  .card-logo {
    height: 32px;
  }
  
  .add-button {
    width: 32px;
    height: 32px;
    border-radius: 50%;
    border: 1px solid #eee;
    background: white;
    color: #666;
    font-size: 20px;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  
  .integration-card h3 {
    font-size: 18px;
    font-weight: bold;
    margin-bottom: 8px;
  }
  
  .integration-card p {
    color: #666;
    line-height: 1.5;
  }
  
  .blog-section {
    background: #000;
    color: white;
    padding: 80px 20px;
    overflow: hidden;
  }
  
  .blog-content {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 60px;
  }
  
  .blog-text {
    flex: 1;
  }
  
  .blog-text h2 {
    font-size: 48px;
    font-weight: bold;
    margin-bottom: 24px;
  }
  
  .blog-text p {
    color: #999;
    margin-bottom: 32px;
    line-height: 1.6;
    max-width: 500px;
  }
  
  .blog-button {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    background: #0066FF;
    color: white;
    padding: 12px 24px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 500;
    transition: background 0.2s;
  }
  
  .blog-button:hover {
    background: #0052cc;
  }
  
  .ebooks-visual {
    position: relative;
    width: 400px;
    height: 400px;
  }
  
  .ebook {
    position: absolute;
    width: 200px;
    height: 280px;
    background: #111;
    border-radius: 8px;
    transform: perspective(1000px) rotateY(-15deg);
    box-shadow: 0 0 30px rgba(0, 102, 255, 0.3);
  }
  
  .ebook-1 {
    top: 60px;
    left: 40px;
  }
  
  .ebook-2 {
    top: 40px;
    left: 140px;
  }
  
  @media (max-width: 768px) {
    .blog-content {
      flex-direction: column;
    }
  
    .blog-text h2 {
      font-size: 36px;
    }
  
    .ebooks-visual {
      width: 100%;
      height: 300px;
    }
  }
  </style>