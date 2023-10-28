<template>
    <div class="portfolio-item">
      <h2>{{ item.title }}</h2>
      <p>{{ item.description }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'PortfolioItem',
    props: {
      item: {
        type: Object,
        required: true
      }
    }
  };
  </script>
  
  <style scoped>
  .portfolio-item {
    margin-bottom: 20px;
  }
  </style>
  