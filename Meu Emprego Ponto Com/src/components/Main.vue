<template>
    <main class="main-content">
      <section class="card-container">
        <div v-for="card in cards" :key="card.id" class="card">
          <img :src="card.image" :alt="card.title" class="card-image" />
          <div class="card-body">
            <h3>{{ card.title }}</h3>
            <p>{{ card.description }}</p>
          </div>
        </div>
      </section>
    </main>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue';
  
  const cards = ref([
    { id: 1, title: 'Card 1', description: 'Descrição do Card 1', image: 'https://via.placeholder.com/150' },
    { id: 2, title: 'Card 2', description: 'Descrição do Card 2', image: 'https://via.placeholder.com/150' },
    { id: 3, title: 'Card 3', description: 'Descrição do Card 3', image: 'https://via.placeholder.com/150' },
    { id: 4, title: 'Card 4', description: 'Descrição do Card 4', image: 'https://via.placeholder.com/150' },
    { id: 5, title: 'Card 5', description: 'Descrição do Card 5', image: 'https://via.placeholder.com/150' },
    { id: 6, title: 'Card 6', description: 'Descrição do Card 6', image: 'https://via.placeholder.com/150' },
    { id: 7, title: 'Card 7', description: 'Descrição do Card 7', image: 'https://via.placeholder.com/150' },
    { id: 8, title: 'Card 8', description: 'Descrição do Card 8', image: 'https://via.placeholder.com/150' },
    { id: 9, title: 'Card 8', description: 'Descrição do Card 8', image: 'https://via.placeholder.com/150' },
    { id: 10, title: 'Card 8', description: 'Descrição do Card 8', image: 'https://via.placeholder.com/150' }
  ]);
  </script>
  
  <style scoped>
  .main-content {
    padding: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }
  
  .card-container {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 20px;
    max-width: 1200px;
    width: 100%;
  }
  
  .card {
    background-color: #f4f4f4;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    overflow: hidden;
    text-align: center;
  }
  
  .card-image {
    width: 100%;
    height: 150px;
    object-fit: cover;
  }
  
  .card-body {
    padding: 15px;
  }
  
  .card-body h3 {
    margin: 10px 0;
    font-size: 1.2rem;
    color: #333;
  }
  
  .card-body p {
    color: #777;
    font-size: 0.9rem;
  }
  </style>
  