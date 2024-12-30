<template>
    <div class="container">
      <!-- FAQ Section -->
      <section class="faq">
        <div class="faq-container">
          <div class="faq-left">
            <h2>Dúvidas<br>frequentes</h2>
            <p>Caso não encontre sua dúvida aqui, acesse nossa central de ajuda ao cliente.</p>
            <button class="help-button">
              <span class="icon">?</span>
              Central de ajuda
            </button>
          </div>
          
          <div class="faq-right">
            <button v-for="(question, index) in questions" 
                    :key="index" 
                    class="question-button">
              <span class="question-number">{{ String(index + 1).padStart(2, '0') }}</span>
              <span class="question-text">{{ question }}</span>
              <span class="chevron">›</span>
            </button>
          </div>
        </div>
      </section>
  
      <!-- Footer -->
      <footer>
        <div class="footer-container">
          <!-- Main Footer Content -->
          <div class="footer-content">
            <!-- Brand Column -->
            <div class="brand-column">
              <!-- <img src="/placeholder.svg?text=kirvano" alt="Kirvano" class="logo" /> -->
              <p>Simples, confiável, lucrativa,<br>para pessoas ambiciosas</p>
              <div class="social-links">
                <a href="#" class="social-button">
                  <!-- <img src="/placeholder.svg?text=in" alt="LinkedIn" /> -->
                </a>
                <a href="#" class="social-button">
                  <!-- <img src="/placeholder.svg?text=yt" alt="YouTube" /> -->
                </a>
                <a href="#" class="social-button">
                  <!-- <img src="/placeholder.svg?text=ig" alt="Instagram" /> -->
                </a>
              </div>
            </div>
  
            <!-- Navigation Columns -->
            <div class="nav-columns">
              <div class="nav-column">
                <h3>Início</h3>
                <a href="#">Área de membros</a>
                <a href="#">Recomência</a>
              </div>
              <div class="nav-column">
                <h3>Funcionalidades</h3>
                <a href="#">Planos e taxas</a>
                <a href="#">Ajuda</a>
              </div>
            </div>
  
            <!-- App Download Column -->
            <div class="app-column">
              <h3>Você pode baixar nosso app</h3>
              <div class="store-buttons">
                <a href="#" class="store-button">
                  <!-- <img src="/placeholder.svg?text=google-play" alt="Google Play" /> -->
                </a>
                <a href="#" class="store-button">
                  <!-- <img src="/placeholder.svg?text=app-store" alt="App Store" /> -->
                </a>
              </div>
            </div>
          </div>
  
          <!-- Footer Bottom -->
          <div class="footer-bottom">
            <p class="company-info">Kirvano Pagamentos LTDA | CNPJ: 48.682.146/0001-19</p>
            <p class="copyright">© Todos os Direitos Reservados</p>
            <div class="legal-links">
              <a href="#">Termos de Uso</a>
              <span class="separator">·</span>
              <a href="#">Política de Privacidade</a>
            </div>
          </div>
        </div>
      </footer>
    </div>
  </template>
  
  <script setup>
  const questions = [
    'Existe alguma cobrança para criar uma conta na Kirvano?',
    'Vendo um produto físico, posso usar a Kirvano?',
    'Para quem é a Kirvano?',
    'Quantos produtos posso vender pela Kirvano?',
    'Qual a taxa para vendas realizadas?'
  ]
  </script>
  
  <style scoped>
* {
  box-sizing: border-box;
}

html, body {
  margin: 0;
  padding: 0;
  overflow-x: hidden; /* Remove a rolagem horizontal */
}

.container {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  max-width: 100%; /* Garante que a largura não ultrapassa a viewport */
  margin: 0;
  padding: 0;
}

/* FAQ Section */
.faq {
  padding: 120px 0;
  background: #fff;
}

.faq-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 24px;
  display: grid;
  grid-template-columns: 1fr 1.5fr;
  gap: 80px;
}

.faq-left h2 {
  font-size: 48px;
  font-weight: 700;
  line-height: 1.1;
  margin-bottom: 24px;
}

.faq-left p {
  color: #666;
  margin-bottom: 32px;
  max-width: 360px;
  line-height: 1.5;
}

.help-button {
  display: inline-flex;
  align-items: center;
  gap: 12px;
  background: #0066FF;
  color: white;
  border: none;
  padding: 12px 24px;
  border-radius: 8px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.2s;
}

.help-button:hover {
  background: #0052cc;
}

.help-button .icon {
  width: 20px;
  height: 20px;
  background: rgba(255,255,255,0.2);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 14px;
}

.question-button {
  width: 100%;
  display: flex;
  align-items: center;
  padding: 24px 0;
  border: none;
  background: none;
  border-bottom: 1px solid #eee;
  cursor: pointer;
  text-align: left;
  transition: all 0.2s;
}

.question-button:hover {
  padding-left: 8px;
}

.question-number {
  color: #0066FF;
  font-weight: 500;
  margin-right: 24px;
  flex-shrink: 0;
}

.question-text {
  flex: 1;
  font-weight: 500;
  color: #111;
}

.chevron {
  color: #0066FF;
  font-size: 24px;
  margin-left: 16px;
  opacity: 0;
  transition: opacity 0.2s;
}

.question-button:hover .chevron {
  opacity: 1;
}

/* Footer Section */
footer {
  background: #000;
  color: white;
  padding: 80px 24px 40px; /* Inclui padding */
  width: 100%; /* Garante largura total */
  position: relative;
  left: 0;
  right: 0;
  box-sizing: border-box; /* Impede estouro de largura */
}

.footer-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 24px;
}

.footer-content {
  display: grid;
  grid-template-columns: 1.2fr 2fr 1.2fr;
  gap: 80px;
  margin-bottom: 80px;
}

.brand-column .logo {
  height: 32px;
  margin-bottom: 24px;
}

.brand-column p {
  font-size: 18px;
  line-height: 1.5;
  margin-bottom: 32px;
}

.social-links {
  display: flex;
  gap: 12px;
}

.social-button {
  width: 40px;
  height: 40px;
  background: #0066FF;
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: background-color 0.2s;
}

.social-button:hover {
  background: #0052cc;
}

.nav-columns {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 80px;
}

.nav-column h3 {
  color: #fff;
  font-size: 16px;
  font-weight: 600;
  margin-bottom: 24px;
}

.nav-column a {
  display: block;
  color: #666;
  text-decoration: none;
  margin-bottom: 16px;
  transition: color 0.2s;
}

.nav-column a:hover {
  color: #fff;
}

.app-column h3 {
  color: #fff;
  font-size: 16px;
  font-weight: 600;
  margin-bottom: 24px;
}

.store-buttons {
  display: flex;
  gap: 16px;
}

.store-button img {
  height: 40px;
}

.footer-bottom {
  padding-top: 40px;
  border-top: 1px solid rgba(255,255,255,0.1);
  color: #666;
  font-size: 14px;
}

.company-info {
  margin-bottom: 8px;
}

.legal-links {
  margin-top: 8px;
}

.legal-links a {
  color: #666;
  text-decoration: none;
  transition: color 0.2s;
}

.legal-links a:hover {
  color: #999;
}

.separator {
  margin: 0 8px;
}

/* Responsiveness */
@media (max-width: 1024px) {
  .faq-container {
    grid-template-columns: 1fr;
    gap: 40px;
  }

  .footer-content {
    grid-template-columns: 1fr;
    gap: 40px;
  }

  .nav-columns {
    gap: 40px;
  }
}

@media (max-width: 640px) {
  .faq-left h2 {
    font-size: 36px;
  }

  .nav-columns {
    grid-template-columns: 1fr;
  }
}

  </style>
  
  