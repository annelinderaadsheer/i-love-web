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
      <img src="/images/Foto-1.JPG" alt="Photo of {name}" class="profile-photo" />
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

  /* Container definition */
  .about-me-container {
    container-type: inline-size;  /* Container query wordt hier ingeschakeld */
    padding: 2rem;
    color: var(--color-dark-pink);
    background-color: var(--color-light-pink);
    display: flex;
    flex-direction: column;
    gap: 2rem;
  }

  .title {
    font-family: 'Abril Fatface', serif;
    font-size: 2rem;
    color: var(--color-red);
    margin-bottom: 1rem;
  }

  .intro-1, .about-me-right p {
    font-family: 'Montserrat', sans-serif;
    font-size: 1rem;
    line-height: 1.6;
    margin-bottom: 1.5rem;
  }

  .photo-container {
    display: flex;
    justify-content: center;
    margin-top: 1rem;
  }

  .profile-photo {
    max-width: 100%;
    height: auto;
    border-radius: 4px;
    border: 2px solid var(--color-dark-pink);
    box-shadow: 0 3px 5px rgba(0, 0, 0, 0.15);
    transition: transform 0.3s, box-shadow 0.3s;
  }

  .profile-photo:hover {
    box-shadow: 0 5px 8px rgba(0, 0, 0, 0.3);
  }

  /* Container Queries voor tekstgroottes en marges */
  @container (min-width: 320px) {
    .intro-1, .about-me-right p {
      font-size: 1rem;
    }
  }

  @container (min-width: 480px) {
    .intro-1, .about-me-right p {
      font-size: 1.1rem;
    }
  }

  @container (min-width: 768px) {
    .intro-1, .about-me-right p {
      font-size: 1.2rem;
    }
  }

  @container (min-width: 1024px) {
    .title {
      font-size: 2.5rem;
    }

    .intro-1, .about-me-right p {
      font-size: 1.3rem;
    }
  }

  @container (min-width: 1280px) {
    .about-me-container {
      padding: 4rem;
    }
    .photo-container {
      width: 60%;
    }

    .title {
      font-size: 3rem;
    }
    .intro-1, .about-me-right p {
      font-size: 1.4rem;
    }
  }

  @container (min-width: 1440px) {
    .about-me-container {
      padding: 4rem;
    }
    .photo-container {
      width: 60%;
    }
    .title {
      font-size: 3.5rem;
    }
    .intro-1, .about-me-right p {
      font-size: 1.5rem;
    }
  }

  @container (min-width: 1920px) {
    .about-me-container {
      padding: 5rem;
    }
    .photo-container {
      width: 50%;
    }
    .title {
      font-size: 4rem;
    }
    .intro-1, .about-me-right p {
      font-size: 1.6rem;
    }
  }

  /* Media Queries voor de lay-out (geen container queries voor layout) */
  @media (min-width: 320px) {
    .about-me-container {
      flex-direction: column;
    }
    .photo-container {
      justify-content: center;
      margin-bottom: 1.5rem;
    }
  }

  @media (min-width: 480px) {
    .about-me-container {
      flex-direction: column;
    }
    .photo-container {
      justify-content: center;
      margin-bottom: 1.5rem;
    }
  }

  @media (min-width: 768px) {
    .about-me-container {
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
    }
    .photo-container {
      margin-right: 2rem;
      width: 85%;
    }
  }

  @media (min-width: 1024px) {
    .about-me-container {
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
      padding: 3rem;
    }
    .photo-container {
      width: 75%;
    }
  }

  @media (min-width: 1280px) {
    .about-me-container {
      padding: 4rem;
    }
    .photo-container {
      width: 60%;
    }
  }

  @media (min-width: 1440px) {
    .about-me-container {
      padding: 4rem;
    }
    .photo-container {
      width: 60%;
    }
  }

  @media (min-width: 1920px) {
    .about-me-container {
      padding: 5rem;
    }
    .photo-container {
      width: 50%;
    }
  }
</style>

