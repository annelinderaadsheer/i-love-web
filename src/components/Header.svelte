<script>
  export let title = "MY PORTFOLIO";
</script>

<header class="header">
  <h1 class="static-text">{title}</h1>
</header>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Abril+Fatface&display=swap');

  .header {
    text-align: center;
    padding: 1rem 5%;
    background-color: var(--color-light-pink);
  }

  .static-text {
    font-size: 2rem;
    font-family: 'Abril Fatface', serif;
    color: var(--color-red);
    opacity: 0;
    transform: scale(0.5); 
    animation: zoomIn 2s ease-out forwards; 
  }

  /* Animatie */
  @keyframes zoomIn {
    0% {
      opacity: 0;
      transform: scale(0.5); 
    }
    50% {
      opacity: 0.8;
      transform: scale(1.1); 
    }
    100% {
      opacity: 1;
      transform: scale(1); 
    }
  }

  /* Media Queries */
  @media (min-width: 320px) {
    .static-text {
      font-size: 3rem; 
    }
  }

  @media (min-width: 480px) {
    .static-text {
      font-size: 4rem;
    }
  }

  @media (min-width: 768px) {
    .static-text {
      font-size: 5rem; 
    }
  }

  @media (min-width: 1024px) {
    .static-text {
      font-size: 6rem; 
    }
  }

  @media (min-width: 1280px) {
    .static-text {
      font-size: 7rem;
    }
  }

  @media (min-width: 1440px) {
    .static-text {
      font-size: 8rem;
    }
  }

  @media (min-width: 1920px) {
    .static-text {
      font-size: 10rem;
    }
  }
</style>