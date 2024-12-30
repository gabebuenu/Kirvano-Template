<template>
    <div class="pricing-container">
      <div class="pricing-header">
        <h2>Planos e taxas</h2>
        <p>Ofereça uma experiência verdadeiramente exclusiva e atraente para os seus membros através das nossas ferramentas de personalização.</p>
      </div>
  
      <div class="pricing-grid">
        <!-- Plano Padrão -->
        <div class="pricing-card dark">
          <div class="pricing-content">
            <h3>Padrão</h3>
            <p>Receba pagamentos de forma simples, com uma plataforma sem custos ocultos.</p>
            <div class="price">4,9% + R$2,00</div>
            <button class="button-primary">Garantir taxa</button>
          </div>
        </div>
  
        <!-- Grandes Contas -->
        <div class="pricing-card light">
          <div class="pricing-content">
            <h3>Grandes contas</h3>
            <p>Se você tem uma operação diferenciada com volume de vendas acima de 100k por mês, podemos ajudá-lo.</p>
            <button class="button-secondary">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                <path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path>
              </svg>
              Falar com gerente de contas
            </button>
          </div>
        </div>
      </div>
  
      <div class="features-grid">
        <!-- Segurança -->
        <div class="feature-card">
          <div class="feature-icon security"></div>
          <h4>Segurança total e conformidade sem concessões</h4>
          <ul>
            <li>Segurança e criptografia de dados</li>
            <li>Certificado PCI DSS</li>
            <li>Segurança para gerenciar suas contas e pagamentos</li>
          </ul>
        </div>
  
        <!-- Saque -->
        <div class="feature-card">
          <div class="feature-icon transfer"></div>
          <h4>Saque enviado para sua conta bancária em minutos</h4>
          <ul>
            <li>Escolha quando você quer receber</li>
            <li>Antecipação automatizada</li>
          </ul>
        </div>
  
        <!-- Métodos de Pagamento -->
        <div class="feature-card">
          <div class="feature-icon payment"></div>
          <h4>Métodos de pagamentos aceitos</h4>
          <ul>
            <li>Cartão de crédito</li>
            <li>PIX</li>
            <li>Boleto</li>
          </ul>
        </div>
  
        <!-- Suporte -->
        <div class="feature-card">
          <div class="feature-icon support"></div>
          <h4>Suporte especializado</h4>
          <ul>
            <li>Velocidade nas soluções</li>
            <li>Atendimento exclusivo e especializado</li>
            <li>Segurança e clareza nas informações</li>
          </ul>
        </div>
  
        <!-- Personalização -->
        <div class="feature-card">
          <div class="feature-icon customize"></div>
          <h4>Personalize a experiência de compra</h4>
          <ul>
            <li>Gatilhos mentais para aumentar a conversão</li>
            <li>Editor de checkout personalizável</li>
          </ul>
        </div>
  
        <!-- Indique e Ganhe -->
        <div class="feature-card">
          <div class="feature-icon referral"></div>
          <h4>+1 Milhão usuários</h4>
          <h5>Indique e ganhe</h5>
          <p>Convide amigos e fique com uma porcentagem sobre as taxas* que a Kirvano receber das vendas do seu contato indicado. Incrível, né?</p>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  .pricing-container {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
    max-width: 1200px;
    margin: 0 auto;
    padding: 60px 20px;
  }
  
  .pricing-header {
    text-align: center;
    margin-bottom: 48px;
  }
  
  .pricing-header h2 {
    font-size: 40px;
    font-weight: bold;
    margin-bottom: 16px;
  }
  
  .pricing-header p {
    color: #666;
    max-width: 600px;
    margin: 0 auto;
  }
  
  .pricing-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 24px;
    margin-bottom: 48px;
  }
  
  .pricing-card {
    border-radius: 12px;
    padding: 32px;
  }
  
  .pricing-card.dark {
    background: #111;
    color: white;
  }
  
  .pricing-card.light {
    background: #fff;
    border: 1px solid #eee;
  }
  
  .pricing-content h3 {
    font-size: 24px;
    font-weight: bold;
    margin-bottom: 16px;
  }
  
  .pricing-content p {
    margin-bottom: 24px;
    line-height: 1.5;
  }
  
  .price {
    font-size: 32px;
    font-weight: bold;
    margin-bottom: 24px;
  }
  
  .button-primary {
    background: #0066FF;
    color: white;
    border: none;
    padding: 12px 24px;
    border-radius: 8px;
    font-weight: 500;
    cursor: pointer;
    width: 100%;
  }
  
  .button-secondary {
    background: #f1f1f1;
    color: #333;
    border: none;
    padding: 12px 24px;
    border-radius: 8px;
    font-weight: 500;
    cursor: pointer;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 8px;
  }
  
  .features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 24px;
  }
  
  .feature-card {
    background: white;
    border-radius: 12px;
    padding: 24px;
    border: 1px solid #eee;
  }
  
  .feature-icon {
    width: 48px;
    height: 48px;
    margin-bottom: 16px;
    background-size: contain;
    background-repeat: no-repeat;
  }
  
  .feature-card h4 {
    font-size: 18px;
    font-weight: bold;
    margin-bottom: 16px;
  }
  
  .feature-card h5 {
    font-size: 16px;
    font-weight: bold;
    margin-bottom: 8px;
  }
  
  .feature-card ul {
    list-style: none;
    padding: 0;
  }
  
  .feature-card li {
    display: flex;
    align-items: center;
    margin-bottom: 8px;
  }
  
  .feature-card li::before {
    content: "";
    display: inline-block;
    width: 16px;
    height: 16px;
    margin-right: 8px;
    background: #0066FF;
    border-radius: 50%;
    flex-shrink: 0;
  }
  
  @media (max-width: 768px) {
    .pricing-header h2 {
      font-size: 32px;
    }
    
    .pricing-grid,
    .features-grid {
      grid-template-columns: 1fr;
    }
  }
  </style>