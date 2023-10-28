<template>
    <div class="home">
      <h1>Welcome to My Portfolio</h1>
      <div class="portfolio-items">
        <PortfolioItem v-for="item in portfolioItems" :key="item.id" :item="item" />
      </div>
    </div>
  </template>
  
  <script>
  import PortfolioItem from '@/components/PortfolioItem.vue';
  
  export default {
    name: 'HomePage',
    components: {
      PortfolioItem
    },
    data() {
      return {
        portfolioItems: [
          { id: 1, title: 'Project 1', description: 'Description of project 1.' },
          { id: 2, title: 'Project 2', description: 'Description of project 2.' },
          // Ajoute plus d'éléments ici si nécessaire
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .home {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .portfolio-items {
    margin-top: 20px;
  }
  </style>
  