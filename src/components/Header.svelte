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
    transition: font-size 0.3s ease;
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