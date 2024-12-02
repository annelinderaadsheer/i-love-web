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
    padding: 2rem 0; /* Vergroot de padding voor meer ruimte rondom de tekst */
    background-color: var(--color-light-pink);
  }

  .static-text {
    font-family: 'Abril Fatface', serif; /* Sierlijk lettertype */
    font-weight: 700;
    color: var(--color-red);
    transition: font-size 0.3s ease;
  }

  /* Responsieve grotere font-groottes */
  @media (min-width: 300px) {
    .static-text {
      font-size: 3rem; /* Groter op kleine schermen */
    }
  }

  @media (min-width: 500px) {
    .static-text {
      font-size: 4rem; /* Groter op middelgrote schermen */
    }
  }

  @media (min-width: 700px) {
    .static-text {
      font-size: 6rem; /* Nog groter op grote schermen */
    }
  }

  @media (min-width: 1000px) {
    .static-text {
      font-size: 8rem; /* Extra groot voor grote schermen */
    }
  }
</style>