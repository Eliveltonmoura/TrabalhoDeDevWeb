
<template>
    <header class="header">
      <div class="logo">
        <h1>Meu Emprego Ponto Com</h1>
      </div>
      <nav class="nav">
        <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/about">Sobre</a></li>
          <li><a href="/contact">Contato</a></li>
        </ul>
      </nav>
      <div class="auth">
        <button @click="handleLogin">{{ isLoggedIn ? 'Logout' : 'Login' }}</button>
      </div>
    </header>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue';
  
  // Variável reativa para estado de login
  const isLoggedIn = ref(false);
  
  // Função para gerenciar o clique no botão de login/logout
  const handleLogin = () => {
    isLoggedIn.value = !isLoggedIn.value;
    if (isLoggedIn.value) {
      alert("Você está logado!");
    } else {
      alert("Você saiu!");
    }
  };
  </script>
  
  <style scoped>
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px;
    background-color: #333;
    color: #fff;
  }
  
  .logo h1 {
    margin: 0;
    font-size: 1.5rem;
  }
  
  .nav ul {
    list-style: none;
    display: flex;
    gap: 15px;
    margin: 0;
    padding: 0;
  }
  
  .nav a {
    color: #fff;
    text-decoration: none;
  }
  
  .auth button {
    padding: 10px 15px;
    background-color: #ff9800;
    border: none;
    border-radius: 5px;
    color: white;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }
  
  .auth button:hover {
    background-color: #e68900;
  }
  </style>
  

