<template>
    <footer class="footer">
      <div class="footer-content">
        <div class="footer-section">
          <h2>Meu Emprego Ponto Com</h2>
          <p>Sua pagina de emprego ou divugação de emprego</p>
        </div>
        
        <div class="footer-section">
          <h3>Links</h3>
          <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/about">Sobre</a></li>
            <li><a href="/contact">Contato</a></li>
            <li><a href="/privacy">Política de Privacidade</a></li>
          </ul>
        </div>
  
        <div class="footer-section">
          <h3>Siga-nos</h3>
          <div class="social-icons">
            <a href="#"><i class="fab fa-facebook-f"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
          </div>
        </div>
      </div>
  
      <div class="footer-bottom">
        <p>&copy; 2024 Todos os direitos reservados.</p>
      </div>
    </footer>
  </template>
  
  <script setup lang="ts">
  </script>
  
  <style scoped>
  .footer {
    background-color: #333;
    color: white;
    padding: 20px 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  
  .footer-content {
    width: 90%;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
  }
  
  .footer-section {
    flex: 1;
    min-width: 200px;
    margin: 10px;
  }
  
  .footer-section h2,
  .footer-section h3 {
    color: #ff9800;
  }
  
  .footer-section p, 
  .footer-section ul {
    margin: 10px 0;
  }
  
  .footer-section ul {
    list-style: none;
    padding: 0;
  }
  
  .footer-section ul li {
    margin: 5px 0;
  }
  
  .footer-section ul li a {
    color: white;
    text-decoration: none;
    transition: color 0.3s;
  }
  
  .footer-section ul li a:hover {
    color: #ff9800;
  }
  
  .social-icons a {
    color: white;
    margin-right: 10px;
    font-size: 1.5rem;
    transition: color 0.3s;
  }
  
  .social-icons a:hover {
    color: #ff9800;
  }
  
  .footer-bottom {
    width: 100%;
    text-align: center;
    margin-top: 20px;
    border-top: 1px solid #444;
    padding-top: 10px;
  }
  </style>
  