<template>
    <section class="steps-section">
      <div class="container">
        <h2 class="section-title">
          Sua primeira venda no digital
          <br />
          mais rápida do que você imagina
        </h2>
  
        <div class="steps-container">
          <div class="steps-list">
            <div class="step active">
              <div class="checkbox">
                <CheckIcon size="20" />
              </div>
              <span>Crie sua conta</span>
            </div>
            <div class="step-content">
              <h3>Cadastro de conta</h3>
              <p>Clique no botão "Cadastre-se". Insira as informações solicitadas e siga o fluxo de boas-vindas.</p>
            </div>
  
            <div class="step">
              <div class="checkbox">
                <CheckIcon size="20" />
              </div>
              <span>Cadastre seu produto</span>
            </div>
            <div class="step-content">
              <h3>Confirmação de e-mail</h3>
              <p>Acesse sua caixa de entrada e clique no link de confirmação para validar seu cadastro.</p>
            </div>
  
            <div class="step">
              <div class="checkbox">
                <CheckIcon size="20" />
              </div>
              <span>Comece a vender</span>
            </div>
            <div class="step-content">
              <h3>Informações complementares</h3>
              <p>Complete seu perfil adicionando informações complementares.</p>
            </div>
          </div>
  
          <div class="browser-preview">
            <div class="browser-header">
              <div class="browser-dots">
                <span class="dot"></span>
                <span class="dot"></span>
                <span class="dot"></span>
              </div>
            </div>
            <div class="browser-content">
              <!-- <img src="/placeholder.svg?height=400&width=500" alt="Kirvano signup form" class="form-preview" /> -->
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  import { CheckIcon } from 'lucide-vue-next'
  </script>
  
  <style>
  .steps-section {
    padding: 120px 0;
    background: #FFFFFF;
  }
  
  .section-title {
    text-align: center;
    font-size: 48px;
    line-height: 1.2;
    font-weight: 800;
    letter-spacing: -0.02em;
    margin-bottom: 80px;
    color: #000000;
  }
  
  .steps-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 80px;
    align-items: flex-start;
    max-width: 1120px;
    margin: 0 auto;
  }
  
  .steps-list {
    display: flex;
    flex-direction: column;
    gap: 32px;
  }
  
  .step {
    display: flex;
    align-items: center;
    gap: 16px;
    font-size: 18px;
    font-weight: 500;
    color: #666666;
  }
  
  .step.active {
    color: #000000;
  }
  
  .checkbox {
    width: 24px;
    height: 24px;
    border-radius: 6px;
    border: 2px solid #EAEAEA;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #CCCCCC;
  }
  
  .step.active .checkbox {
    background: #0066FF;
    border-color: #0066FF;
    color: #FFFFFF;
  }
  
  .step-content {
    padding-left: 40px;
  }
  
  .step-content h3 {
    font-size: 20px;
    font-weight: 600;
    color: #000000;
    margin-bottom: 8px;
  }
  
  .step-content p {
    font-size: 16px;
    color: #666666;
    line-height: 1.5;
  }
  
  .browser-preview {
    background: #FFFFFF;
    border-radius: 8px;
    box-shadow: 0 4px 24px rgba(0, 0, 0, 0.08);
    overflow: hidden;
  }
  
  .browser-header {
    background: #F5F5F5;
    padding: 12px 16px;
    border-bottom: 1px solid #EAEAEA;
  }
  
  .browser-dots {
    display: flex;
    gap: 8px;
  }
  
  .dot {
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background: #DDDDDD;
  }
  
  .dot:nth-child(1) { background: #FF5F57; }
  .dot:nth-child(2) { background: #FFBD2E; }
  .dot:nth-child(3) { background: #28C840; }
  
  .browser-content {
    padding: 24px;
  }
  
  .form-preview {
    width: 100%;
    height: auto;
  }
  
  @media (max-width: 1024px) {
    .section-title {
      font-size: 40px;
    }
  
    .steps-container {
      gap: 40px;
    }
  }
  
  @media (max-width: 768px) {
    .steps-container {
      grid-template-columns: 1fr;
    }
  
    .browser-preview {
      max-width: 500px;
      margin: 0 auto;
    }
  }
  
  @media (max-width: 640px) {
    .section-title {
      font-size: 32px;
    }
  
    .step {
      font-size: 16px;
    }
  
    .step-content h3 {
      font-size: 18px;
    }
  }
  </style>