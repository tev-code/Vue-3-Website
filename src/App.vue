<script setup>
import Header from './components/Header.vue'
import Home from './views/Home.vue'
</script>

<template>
<div class="app">
  <Header/>
  <vue-router/>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400&display=swap');

  :root { 

  --font-medium: 500;
   }

  :root {
    --first-color: #000000;
    --secondary-color: #3dac63;
    --white-color: #bcaad1;
    --dark-color: #3700B3;
    --text-color: #ffffff;
   }

  :root {
     --body-font: 'Poppins', sans-serif;;
     --big-font-size: 6.25rem;
     --h2-font-size: 1.25rem;
     --normal-size: 938rem;
     --small-font-size: 875rem; 
   }

  @media screen and (min-width: 768px){
    :root {
        --big-font-size: 10.5rem;
        --h2-font-size: 2rem;
        --normal-size: 1rem;
        --small-font-size: 875rem; 
    }
}

*,::before, ::after{
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    margin: var(--header-height) 0 0 0;
    font-family: var(--body-font);
    font-size: var(--normal-font-size);
    font-weight: var(--font-medium);
    color: var(--text-color);
    line-height: 1.6;
}

h1,h2,p {
    margin: 0;
}





</style>
