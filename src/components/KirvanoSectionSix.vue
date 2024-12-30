<template>
    <div class="container">
      <div class="header">
        <h1>Na Kirvano você pode mais</h1>
        <p>Com nossa plataforma você tem total controle do seu negócio.</p>
      </div>
  
      <div class="cards">
        <div class="card">
          <div class="icon">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M7 10L12 15L17 10" stroke="#0066FF" stroke-width="2"/>
            </svg>
          </div>
          <h3>Upsell, downsell, cross sell</h3>
          <p>Aproveite ao máximo cada oportunidade de venda e aumente seus lucros.</p>
        </div>
  
        <div class="card">
          <div class="icon">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <circle cx="12" cy="12" r="9" stroke="#0066FF" stroke-width="2"/>
              <path d="M12 8V12L15 15" stroke="#0066FF" stroke-width="2"/>
            </svg>
          </div>
          <h3>Recuperador de vendas</h3>
          <p>Envie mensagens relevantes para seus clientes, aumentando a chance de conversão.</p>
        </div>
      </div>
  
      <div class="cta">
        <div class="cta-content">
          <h2>Comece de forma gratuita</h2>
          <p>Venda seus produtos e serviços digitais e receba através da Kirvano.</p>
          <button>Cadastre-se</button>
        </div>
        <div class="cta-image">
          <!-- <img src="/placeholder.svg?height=200&width=200" alt="Ilustração"> -->
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  body {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  }
  
  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 40px 20px;
  }
  
  .header {
    text-align: center;
    margin-bottom: 60px;
  }
  
  .header h1 {
    font-size: 48px;
    font-weight: bold;
    margin-bottom: 16px;
    color: #111;
  }
  
  .header p {
    font-size: 18px;
    color: #666;
  }
  
  .cards {
    display: flex;
    gap: 24px;
    margin-bottom: 40px;
    justify-content: center;
  }
  
  .card {
    background: #fff;
    padding: 32px;
    border-radius: 8px;
    box-shadow: 0 1px 3px rgba(0,0,0,0.1);
    flex: 1;
    max-width: 400px;
  }
  
  .icon {
    margin-bottom: 24px;
  }
  
  .card h3 {
    font-size: 20px;
    font-weight: 600;
    margin-bottom: 16px;
    color: #111;
  }
  
  .card p {
    color: #666;
    line-height: 1.5;
  }
  
  .cta {
    background: #111;
    border-radius: 16px;
    padding: 48px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-top: 60px;
  }
  
  .cta-content {
    flex: 1;
    padding-right: 48px;
  }
  
  .cta h2 {
    color: #fff;
    font-size: 36px;
    font-weight: bold;
    margin-bottom: 16px;
  }
  
  .cta p {
    color: #999;
    margin-bottom: 24px;
  }
  
  .cta button {
    background: #0066FF;
    color: white;
    border: none;
    padding: 12px 24px;
    border-radius: 8px;
    font-size: 16px;
    font-weight: 500;
    cursor: pointer;
    transition: background 0.2s;
  }
  
  .cta button:hover {
    background: #0052cc;
  }
  
  .cta-image {
    flex: 0 0 300px;
  }
  
  .cta-image img {
    width: 100%;
    height: auto;
  }
  
  @media (max-width: 768px) {
    .cards {
      flex-direction: column;
    }
    
    .cta {
      flex-direction: column;
      text-align: center;
      padding: 32px;
    }
    
    .cta-content {
      padding-right: 0;
      margin-bottom: 32px;
    }
    
    .cta-image {
      flex: 0 0 auto;
      width: 100%;
      max-width: 300px;
      margin: 0 auto;
    }
    
    .header h1 {
      font-size: 36px;
    }
  }
  </style>