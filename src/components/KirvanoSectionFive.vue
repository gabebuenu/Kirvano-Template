<template>
    <section class="affiliate-section">
      <div class="container">
        <div class="affiliate-content">
          <div class="text-center">
            <h2>
              Monte seu negócio digital
              <br />
              sem um produto próprio
            </h2>
            <p>
              Promova produtos de terceiros através de links de afiliação e receba uma
              <br />
              comissão por cada venda realizada.
            </p>
          </div>
  
          <div class="browser-window">
            <div class="browser-header">
              <div class="browser-controls">
                <span class="dot red"></span>
                <span class="dot yellow"></span>
                <span class="dot green"></span>
              </div>
              <div class="browser-address">
                <!-- <img src="/placeholder.svg?height=20&width=20" alt="Kirvano" class="browser-icon" /> -->
                <span>kirvano</span>
              </div>
            </div>
            <div class="browser-content">
              <div class="affiliate-invite">
                <div class="invite-header">
                  <h3>Você foi convidado a se tornar afiliado desse produto e ganhar dinheiro com ele</h3>
                </div>
                <div class="product-preview">
                  <div class="product-image">
                    <!-- <img src="/placeholder.svg?height=60&width=60" alt="Product" /> -->
                  </div>
                  <div class="product-info">
                    <span class="product-name">Nome do produto</span>
                    <span class="product-price">Por R$ 99,90</span>
                  </div>
                  <button class="affiliate-button">
                    Fazer parte e gerar seu link
                  </button>
                </div>
                <div class="invite-footer">
                  <span>Informações gerais</span>
                  <div class="info-grid">
                    <div class="info-item">Produto</div>
                    <div class="info-item">Taxa Cobrada</div>
                    <div class="info-item">Pago</div>
                    <div class="info-item">...</div>
                  </div>
                </div>
              </div>
            </div>
          </div>
  
            <div class="notification-container">
                <div class="notification-wrapper">
                    <img 
                    :src="'https://www.kirvano.com/images/Mockups_Notificações_1-2-1.gif'" 
                    alt="Notifications"
                    class="notifications-gif"
                    />
                </div>
            </div>
        </div>
      </div>
    </section>
  </template>
  
  <style>
  .affiliate-section {
    background: #000000;
    padding: 120px 0;
    color: white;
    overflow: hidden;
  }
  
  .container {
    max-width: 1240px;
    margin: 0 auto;
    padding: 0 24px;
  }
  
  .affiliate-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 64px;
  }
  
  .text-center {
    text-align: center;
  }
  
  h2 {
    font-size: 48px;
    font-weight: 800;
    line-height: 1.1;
    letter-spacing: -0.02em;
    margin-bottom: 24px;
  }
  
  p {
    font-size: 20px;
    line-height: 1.5;
    color: #999999;
  }
  
  .browser-window {
    width: 100%;
    max-width: 800px;
    background: white;
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 24px 48px rgba(0, 0, 0, 0.2);
  }
  
  .browser-header {
    background: #F5F5F5;
    padding: 16px;
    display: flex;
    align-items: center;
    border-bottom: 1px solid #EAEAEA;
  }
  
  .browser-controls {
    display: flex;
    gap: 8px;
    margin-right: 16px;
  }
  
  .dot {
    width: 12px;
    height: 12px;
    border-radius: 50%;
  }
  
  .dot.red { background: #FF5F57; }
  .dot.yellow { background: #FFBD2E; }
  .dot.green { background: #28C840; }
  
  .browser-address {
    display: flex;
    align-items: center;
    gap: 8px;
    padding: 6px 12px;
    background: #FFFFFF;
    border-radius: 6px;
    color: #666666;
    font-size: 14px;
  }
  
  .browser-icon {
    width: 16px;
    height: 16px;
    border-radius: 4px;
  }
  
  .browser-content {
    padding: 32px;
  }
  
  .affiliate-invite {
    color: #000000;
  }
  
  .invite-header {
    margin-bottom: 24px;
  }
  
  .invite-header h3 {
    font-size: 24px;
    font-weight: 600;
    line-height: 1.3;
  }
  
  .product-preview {
    display: flex;
    align-items: center;
    gap: 16px;
    padding: 16px;
    background: #F8F8F8;
    border-radius: 8px;
    margin-bottom: 24px;
  }
  
  .product-image img {
    width: 60px;
    height: 60px;
    border-radius: 8px;
    object-fit: cover;
  }
  
  .product-info {
    flex-grow: 1;
    display: flex;
    flex-direction: column;
    gap: 4px;
  }
  
  .product-name {
    font-weight: 500;
    color: #333333;
  }
  
  .product-price {
    font-size: 14px;
    color: #666666;
  }
  
  .affiliate-button {
    background: #0066FF;
    color: white;
    border: none;
    padding: 12px 24px;
    border-radius: 4px;
    font-weight: 500;
    cursor: pointer;
    white-space: nowrap;
  }
  
  .invite-footer {
    color: #666666;
  }
  
  .info-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 16px;
    margin-top: 12px;
    font-size: 14px;
  }
  
  .notification-container {
    width: 100%;
    max-width: 1000px;
    margin: 0 auto;
    position: relative;
  }
  
  .notifications-gif {
    width: 100%;
    height: auto;
    display: block;
  }
  
  @media (max-width: 768px) {
    h2 {
      font-size: 36px;
    }
  
    p {
      font-size: 18px;
    }
  
    p br {
      display: none;
    }
  
    .browser-window {
      margin: 0 -24px;
      border-radius: 0;
    }
  
    .product-preview {
      flex-direction: column;
      text-align: center;
    }
  
    .info-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }
  
  @media (max-width: 640px) {
    h2 {
      font-size: 32px;
    }
  
    .browser-content {
      padding: 24px 16px;
    }
  
    .invite-header h3 {
      font-size: 20px;
    }
  }

  /* css alterado */

  .notification-container {
  width: 100%;
  max-width: 1000px;
  margin: 0 auto;
  position: relative;
  padding: 0 24px;
}

.notification-wrapper {
  border-radius: 16px;
  overflow: hidden; /* This ensures the gif respects the border radius */
  box-shadow: 0 24px 48px rgba(0, 0, 0, 0.2);
}

.notifications-gif {
  width: 100%;
  height: auto;
  display: block;
  vertical-align: middle; /* Removes any potential bottom spacing */
}
  </style>