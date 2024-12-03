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

  /* Media Queries */
  @media (min-width: 300px) {
    .about-me-container {
      flex-direction: column;
    }
    .photo-container {
      justify-content: center;
      margin-bottom: 1.5rem;
    }
    .profile-photo {
      max-width: 100%;
    }
    .intro-1, .about-me-right p {
      font-size: 1rem;
    }
  }

  @media (min-width: 500px) {
    .about-me-container {
      flex-direction: column;
    }
    .photo-container {
      justify-content: center;
      margin-bottom: 1.5rem;
    }
    .profile-photo {
      max-width: 100%;
    }
    .intro-1, .about-me-right p {
      font-size: 1.2rem;
    }
  }

  @media (min-width: 700px) {
    .about-me-container {
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
    }
    .photo-container {
      margin-right: 2rem;
      width: 85%;
    }
    .profile-photo {
      max-width: 100%; 
    }
    .intro-1, .about-me-right p {
      font-size: 1.2rem;
    }
  }

  @media (min-width: 1000px) {
    .about-me-container {
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
      padding: 3rem;
    }
    .photo-container {
      width: 75%;
    }
    .title {
      font-size: 2.5rem;
    }
    .intro-1, .about-me-right p {
      font-size: 1.2rem;
    }
  }
</style>