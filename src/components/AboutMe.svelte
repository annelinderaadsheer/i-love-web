<script>
  export let name = "Annelinde";
  export let github = "https://github.com/annelinderaadsheer";
  export let linkedin = "https://www.linkedin.com/in/annelinde-raadsheer-b38375194/";
  export let email = "anne_linde@live.nl";
</script>

<section class="about-me-container">
  <header>
    <h2 class="title">ABOUT ME</h2>
    <p class="intro-1">
      Hi there! My name is {name}, and I'm a frontend developer with love for creating responsive and accessible websites.
    </p>
    <div class="photo-container">
      <img src="/images/photo1.jpg" alt="Photo 1 of {name}" class="profile-photo" />
      <img src="/images/photo2.jpg" alt="Photo 2 of {name}" class="profile-photo" />
    </div>
    <p>
      <strong class="intro-2">
        LET'S CREATE SOMETHING TOGETHER!
      </strong>
    </p>
    <div class="about-me-buttons">
      <a href={github} target="_blank" class="button github">GitHub</a>
      <a href={linkedin} target="_blank" class="button linkedin">LinkedIn</a>
      <a href={"mailto:" + email} class="button email">E-mail</a>
    </div>
  </header>

  <section class="about-me-right">
    <h2 class="title">WHAT IS A FRONTEND DEVELOPER?</h2>
    <p>
      As a frontend developer, I am passionate about creating user-friendly websites.
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

  /* Titels met Abril Fatface */
  .title {
    font-family: 'Abril Fatface', serif;
    font-size: 2rem;
    color: var(--color-red);
  }

  /* Kleine teksten met Montserrat */
  .intro-1, .about-me-right p {
    font-family: 'Montserrat', sans-serif;
    font-size: 1rem;
    line-height: 1.6;
  }

  .photo-container {
    justify-content: center;
  }

  .profile-photo {
    max-width: 40%;
    border-radius: 2px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  }

  .about-me-buttons {
    display: flex;
    gap: 1rem;
    margin-top: 1rem;
  }

  .button {
    text-decoration: none;
    padding: 0.5rem 1rem;
    border-radius: 4px;
    color: var(--color-red);
    background-color: var(--color-white);
    border: 2px solid var(--color-dark-pink);
    transition: background-color 0.3s;
    font-family: 'Montserrat', sans-serif;
    box-shadow: 0 3px 5px rgba(0, 0, 0, 0.15);
  }

  .button:hover {
    background-color: var(--color-dark-pink);
    color: var(--color-light-pink);
    box-shadow: 0 5px 8px rgba(0, 0, 0, 0.2);
    transform: translateY(-2px);
  }

  /* Styling for static text */
  .intro-2 {
    font-weight: bold;
    font-family: 'Montserrat', sans-serif;
    color: var(--color-red);
  }
</style>
