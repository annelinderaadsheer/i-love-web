<script>
  export let title = "MY PORTFOLIO";
</script>

<header class="header">
  <h1 class="static-text">{title}</h1>
</header>

<style>
  .header {
    text-align: center;
    padding: 1.5rem 0;
    container-type: inline-size; 
    background-color: var(--color-light-pink);
  }

  .static-text {
    font-variation-settings: 'wght' 700;
    transition: font-size 0.3s ease; 
    color: var(--color-red);
  }

  @container (min-width: 300px) {
    .static-text {
      font-size: 1.5rem; 
    }
  }

  @container (min-width: 500px) {
    .static-text {
      font-size: 2rem; 
    }
  }

  @container (min-width: 700px) {
    .static-text {
      font-size: 4rem; 
    }
  }
</style>
