<script>
  export let title = "MY PORTFOLIO";
</script>

<header class="header">
  <h1 class="animated-text">{title}</h1>
</header>

<style>
  .header {
    text-align: center;
    padding: 1.5rem 0;
    /* display: block; */
    container-type: inline-size; 
  }

  .animated-text {
    font-variation-settings: 'wght' 700;
    animation: fontAnimation 6s infinite ease-in-out;
    transition: font-size 0.3s ease; 
  }

  @keyframes fontAnimation {
    0% {
      font-variation-settings: 'wght' 700;
      transform: scale(1);
    }
    50% {
      font-variation-settings: 'wght' 700;
      transform: scale(1.1);
    }
    100% {
      font-variation-settings: 'wght' 700;
      transform: scale(1.2);
    }
  }

  @container (min-width: 300px) {
    .animated-text {
      font-size: 1.5rem; 
    }
  }

  @container (min-width: 500px) {
    .animated-text {
      font-size: 2rem; 
    }
  }

  @container (min-width: 700px) {
    .animated-text {
      font-size: 4rem; 
    }
  }
</style>