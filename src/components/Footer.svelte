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
  }

  .button:hover {
    background-color: var(--color-grey);
    color: var(--color-red);
    box-shadow: 0 5px 8px rgba(0, 0, 0, 0.3);
    transform: translateY(-2px) scale(1.05);
  }
</style>
