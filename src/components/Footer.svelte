<script>
  export let github = "https://github.com/annelinderaadsheer";
  export let linkedin = "https://www.linkedin.com/in/annelinde-raadsheer-b38375194/";
  export let email = "anne_linde@live.nl";
</script>

<footer class="footer">
  <p class="intro-2">
    LET'S CREATE SOMETHING TOGETHER!
  </p>
  <div class="about-me-buttons">
    <a href={github} target="_blank" class="button github">GitHub</a>
    <a href={linkedin} target="_blank" class="button linkedin">LinkedIn</a>
    <a href={"mailto:" + email} class="button email">E-mail</a>
  </div>
</footer>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Abril+Fatface&family=Montserrat:wght@400;700&display=swap');

  .footer {
    text-align: center;
    padding: 2rem 0;
    background-color: var(--color-light-pink);
    border-top: 2px solid var(--color-dark-pink);
  }

  .intro-2 {
    font-weight: bold;
    font-family: 'Montserrat', sans-serif;
    color: var(--color-red);
    margin-bottom: 1rem;
    font-size: 1.2rem; /* Standaard tekstgrootte voor intro-2 */
  }

  .about-me-buttons {
    display: flex;
    justify-content: center;
    gap: 1rem;
  }

  .button {
    text-decoration: none;
    padding: 0.5rem 1rem;
    border-radius: 4px;
    color: var(--color-red);
    background-color: var(--color-white);
    border: 2px solid var(--color-dark-pink);
    transition: background-color 0.3s, transform 0.2s ease, box-shadow 0.3s;
    font-family: 'Montserrat', sans-serif;
    box-shadow: 0 3px 5px rgba(0, 0, 0, 0.15);
    font-size: 1rem;
    font-weight: bold;
  }

  .button:hover {
    background-color: var(--color-grey);
    color: var(--color-red);
    box-shadow: 0 5px 8px rgba(0, 0, 0, 0.3);
    transform: translateY(-2px) scale(1.05);
  }

  /* Media Queries */
  @media (min-width: 320px) {
    .footer {
      padding: 2rem 0;
    }

    .intro-2 {
      font-size: 1.2rem;
    }

    .button {
      font-size: 1rem;
      padding: 0.5rem 1rem;
    }
  }

  @media (min-width: 480px) {
    .footer {
      padding: 2.5rem 0;
    }

    .intro-2 {
      font-size: 1.3rem;
    }

    .button {
      font-size: 1.1rem;
      padding: 0.6rem 1.2rem;
    }
  }

  @media (min-width: 768px) {
    .footer {
      padding: 3rem 0;
    }

    .intro-2 {
      font-size: 1.5rem;
    }

    .button {
      font-size: 1.2rem;
      padding: 0.7rem 1.4rem;
    }
  }

  @media (min-width: 1024px) {
    .footer {
      padding: 3.5rem 0;
    }

    .intro-2 {
      font-size: 1.7rem;
    }

    .button {
      font-size: 1.3rem;
      padding: 0.8rem 1.6rem;
    }
  }

  @media (min-width: 1280px) {
    .footer {
      padding: 4rem 0;
    }

    .intro-2 {
      font-size: 1.8rem;
    }

    .button {
      font-size: 1.4rem;
      padding: 0.9rem 1.8rem;
    }
  }

  @media (min-width: 1440px) {
    .footer {
      padding: 4.5rem 0;
    }

    .intro-2 {
      font-size: 2rem;
    }

    .button {
      font-size: 1.5rem;
      padding: 1rem 2rem;
    }
  }

  @media (min-width: 1920px) {
    .footer {
      padding: 5rem 0;
    }

    .intro-2 {
      font-size: 2.2rem;
    }

    .button {
      font-size: 1.6rem;
      padding: 1.1rem 2.2rem;
    }
  }
</style>
