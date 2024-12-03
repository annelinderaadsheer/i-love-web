<script>
  export let name = "Annelinde";
</script>

<section class="about-me-container">
  <header>
    <h2 class="title">ABOUT ME</h2>
    <p class="intro-1">
      Hi there! My name is {name}, and I'm a 24-year-old frontend developer based in Amsterdam. I’m currently studying FDND at the HvA. When I’m not coding, you’ll find me staying active through sports, exploring new destinations, or experimenting in the kitchen with delicious recipes.
    </p>
    <div class="photo-container">
      <img src="/images/Foto-1.JPG" alt="Photo 1 of {name}" class="profile-photo" />
    </div>
  </header>

  <section class="about-me-right">
    <h2 class="title">WHAT IS A FRONTEND DEVELOPER?</h2>
    <p>
      As a frontend developer, I bring ideas into real life in the browser. By combining creativity and code, I build websites that are progressively enhanced, responsive, and accessible to everyone.
    </p>
  </section>
</section>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Abril+Fatface&family=Montserrat:wght@400;700&display=swap');

  .about-me-container {
    display: flex;
    flex-wrap: wrap;
    padding: 2rem;
    color: var(--color-dark-pink);
    background-color: var(--color-light-pink);
  }

  .title {
    font-family: 'Abril Fatface', serif;
    font-size: 2rem;
    color: var(--color-red);
  }

  .intro-1, .about-me-right p {
    font-family: 'Montserrat', sans-serif;
    font-size: 1rem;
    line-height: 1.6;
  }

  .photo-container {
    justify-content: center;
  }

  .profile-photo {
    max-width: 100%;
    border-radius: 4px;
    border: 2px solid var(--color-dark-pink); 
    box-shadow: 0 3px 5px rgba(0, 0, 0, 0.15);
    transition: transform 0.3s, box-shadow 0.3s;
  }

  .profile-photo:hover {
    box-shadow: 0 5px 8px rgba(0, 0, 0, 0.3); 
  }
</style>
