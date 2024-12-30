<template>
    <div>
      <!-- Services Section -->
      <section class="services-section">
        <div class="container">
          <div class="services-content">
            <div class="services-text">
              <div class="title-group">
                <h2>Criou algo fantástico?</h2>
                <h3>Te ajudamos a vender.</h3>
              </div>
              
              <div class="services-grid">
                <div v-for="service in services" :key="service" class="service-tag">
                  <div class="checkbox">
                    <div class="checkbox-inner"></div>
                  </div>
                  {{ service }}
                </div>
              </div>
            </div>
            <div class="services-illustration">
              <!-- <img src="/placeholder.svg?height=300&width=300" alt="Services illustration" /> -->
            </div>
          </div>
        </div>
      </section>
  
      <!-- Payments Section -->
      <section class="payments-section">
        <div class="container">
          <div class="payments-content">
            <div class="payments-text">
              <h2>Pagamentos<br>recorrentes facilitados</h2>
              <p>Aprove suas vendas personalizando planos com datas flexíveis de pagamento para melhorar a experiência dos seus clientes.</p>
              <button class="cta-button">
                Criar assinatura
              </button>
            </div>
            <div class="payments-illustration">
              <!-- <img src="/placeholder.svg?height=400&width=400" alt="Payments illustration" /> -->
            </div>
          </div>
        </div>
      </section>
  
      <!-- Sales Recovery Section -->
      <section class="recovery-section">
        <div class="container">
          <div class="recovery-content">
            <div class="recovery-left">
              <h2>Recuperador de<br>vendas nativo</h2>
              <p>Fale com seu cliente incapaz de pagar em dia, nosso recuperador envia mensagens relevantes para os seus clientes, o que aumenta a taxa de conversão.</p>
              
              <div class="communication-methods">
                <div class="method">
                  <Mail class="icon" size="18" />
                  <span>Email</span>
                </div>
                <div class="method">
                  <MessageSquare class="icon" size="18" />
                  <span>SMS</span>
                </div>
                <div class="method">
                  <MessageCircle class="icon" size="18" />
                  <span>WhatsApp</span>
                </div>
              </div>
  
              <div class="chat-preview">
                <div v-for="message in messages" :key="message.text" class="message-item">
                  <div class="message-dot" :class="message.status"></div>
                  <span class="message-text">{{ message.text }}</span>
                  <span class="time">{{ message.time }}</span>
                </div>
              </div>
            </div>
  
            <div class="recovery-right">
              <h3>Alta taxa de conversão</h3>
              <p>Nosso sistema de checkout rápido e eficiente facilita a compra para todos os clientes, apresentando a taxa de conversão da tabela de resultados de pagamentos.</p>
              
              <div class="conversion-rates">
                <div v-for="rate in rates" :key="rate.value" class="rate-circle">
                  <svg viewBox="0 0 36 36">
                    <path 
                      d="M18 2.0845a 15.9155 15.9155 0 0 1 0 31.831a 15.9155 15.9155 0 0 1 0 -31.831"
                      :stroke-dasharray="`${rate.value}, 100`"
                    />
                  </svg>
                  <span>{{ rate.value }}%</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>
  </template>
  
  <script setup>
  import { Mail, MessageSquare, MessageCircle } from 'lucide-vue-next'
  
  const services = [
    'Fotografia',
    'Mentorias',
    'Cursos Online',
    'Aulas',
    'Comunidade',
    'Assinatura',
    'E-Books',
    'Newsletter',
    'Freelances',
    'Consultas'
  ]
  
  const messages = [
    { text: 'Cobrança criada para João Carlos', time: 'Há 2 minutos', status: 'blue' },
    { text: 'Mensagem enviada', time: 'Há 1 minuto', status: 'blue' },
    { text: 'Mensagem visualizada', time: 'Agora', status: 'blue' },
    { text: 'Pagamento aprovado', time: 'Agora', status: 'green' }
  ]
  
  const rates = [
    { value: 85 },
    { value: 90 },
    { value: 95 }
  ]
  </script>
  
  <style>
  /* Base Styles */
  .container {
    max-width: 1240px;
    margin: 0 auto;
    padding: 0 24px;
  }
  
  /* Services Section */
  .services-section {
    background: #000000;
    padding: 80px 0;
    color: white;
    border-radius: 16px;
    margin: 24px auto; /* Centraliza horizontalmente */
    max-width: 1200px;  /* Reduz o tamanho horizontal */
}
  
  .services-content {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    gap: 80px;
  }
  
  .title-group {
    margin-bottom: 48px;
  }
  
  .services-text h2 {
    font-size: 48px;
    font-weight: 800;
    line-height: 1.1;
    margin-bottom: 8px;
  }
  
  .services-text h3 {
    font-size: 48px;
    font-weight: 800;
    line-height: 1.1;
    color: #FFFFFF;
  }
  
  .services-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 12px;
    max-width: 520px;
  }
  
  .service-tag {
    display: flex;
    align-items: center;
    gap: 10px;
    background: rgba(255, 255, 255, 0.1);
    padding: 10px 16px;
    border-radius: 8px;
    font-size: 14px;
    font-weight: 500;
  }
  
  .checkbox {
    width: 18px;
    height: 18px;
    border: 2px solid rgba(255, 255, 255, 0.2);
    border-radius: 4px;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
  }
  
  .checkbox-inner {
    width: 10px;
    height: 10px;
    background: #0066FF;
    border-radius: 2px;
  }
  
  .services-illustration {
    flex-shrink: 0;
    margin-top: -40px;
  }
  
  .services-illustration img {
    width: 360px;
    height: auto;
  }
  
  /* Payments Section */
  .payments-section {
    background: #000000;
    padding: 120px 0;
    color: white;
  }
  
  .payments-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 80px;
  }
  
  .payments-text {
    max-width: 520px;
  }
  
  .payments-text h2 {
    font-size: 48px;
    font-weight: 800;
    line-height: 1.1;
    margin-bottom: 24px;
  }
  
  .payments-text p {
    font-size: 18px;
    line-height: 1.6;
    color: #999999;
    margin-bottom: 32px;
  }
  
  .cta-button {
    background: #0066FF;
    color: white;
    border: none;
    padding: 16px 32px;
    border-radius: 4px;
    font-size: 16px;
    font-weight: 500;
    cursor: pointer;
    transition: background-color 0.2s;
  }
  
  .cta-button:hover {
    background: #0052CC;
  }
  
  /* Recovery Section */
  .recovery-section {
    background: #FFFFFF;
    padding: 120px 0;
  }
  
  .recovery-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 80px;
    align-items: start;
  }
  
  .recovery-left h2 {
    font-size: 40px;
    font-weight: 800;
    line-height: 1.1;
    margin-bottom: 24px;
    letter-spacing: -0.02em;
  }
  
  .recovery-left p {
    font-size: 16px;
    line-height: 1.6;
    color: #666666;
    margin-bottom: 40px;
    max-width: 480px;
  }
  
  .communication-methods {
    display: flex;
    gap: 32px;
    margin-bottom: 40px;
  }
  
  .method {
    display: flex;
    align-items: center;
    gap: 8px;
    color: #666666;
    font-size: 14px;
  }
  
  .method .icon {
    color: #999999;
  }
  
  .chat-preview {
    background: #FFFFFF;
    border-radius: 12px;
    padding: 24px;
    box-shadow: 0 4px 24px rgba(0, 0, 0, 0.06);
  }
  
  .message-item {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 12px 0;
    border-bottom: 1px solid #F5F5F5;
  }
  
  .message-item:last-child {
    border-bottom: none;
  }
  
  .message-dot {
    width: 8px;
    height: 8px;
    border-radius: 50%;
    flex-shrink: 0;
  }
  
  .message-dot.blue {
    background: #0066FF;
  }
  
  .message-dot.green {
    background: #00CC66;
  }
  
  .message-text {
    font-size: 14px;
    color: #333333;
    flex-grow: 1;
  }
  
  .time {
    font-size: 14px;
    color: #999999;
  }
  
  .recovery-right h3 {
    font-size: 40px;
    font-weight: 800;
    line-height: 1.1;
    margin-bottom: 24px;
    letter-spacing: -0.02em;
  }
  
  .recovery-right p {
    font-size: 16px;
    line-height: 1.6;
    color: #666666;
    margin-bottom: 48px;
    max-width: 480px;
  }
  
  .conversion-rates {
    display: flex;
    gap: 40px;
  }
  
  .rate-circle {
    position: relative;
    width: 100px;
    height: 100px;
  }
  
  .rate-circle svg {
    width: 100%;
    height: 100%;
    transform: rotate(-90deg);
  }
  
  .rate-circle path {
    fill: none;
    stroke: #0066FF;
    stroke-width: 2.5;
  }
  
  .rate-circle span {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 20px;
    font-weight: 600;
    color: #333333;
  }
  
  @media (max-width: 1200px) {
    .services-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }
  
  @media (max-width: 1024px) {
    .services-text h2,
    .services-text h3,
    .payments-text h2,
    .recovery-left h2,
    .recovery-right h3 {
      font-size: 40px;
    }
  }
  
  @media (max-width: 768px) {
    .services-content,
    .payments-content {
      flex-direction: column;
    }
  
    .recovery-content {
      grid-template-columns: 1fr;
    }
  
    .services-illustration {
      margin-top: 0;
      order: -1;
    }
  
    .services-illustration img {
      width: 100%;
      max-width: 360px;
    }
  }
  
  @media (max-width: 640px) {
    .services-text h2,
    .services-text h3,
    .payments-text h2,
    .recovery-left h2,
    .recovery-right h3 {
      font-size: 32px;
    }
  
    .services-grid {
      grid-template-columns: 1fr;
    }
  
    .communication-methods {
      flex-direction: column;
      gap: 16px;
    }
  
    .conversion-rates {
      gap: 24px;
    }
  
    .rate-circle {
      width: 80px;
      height: 80px;
    }
  }
  </style>