<script>
  export let name = "Annelinde";
  export let github = "https://github.com/annelinderaadsheer";
  export let linkedin = "https://www.linkedin.com/in/annelinde-raadsheer-b38375194/";
  export let email = "anne_linde@live.nl";

  // Typen animatie
  import { onMount } from 'svelte';

  let typedText = "";

  onMount(() => {
    let text = "LET'S CREATE SOMETHING TOGETHER.";
    let index = 0;
    const interval = setInterval(() => {
      typedText += text[index];
      index++;
      if (index === text.length) {
        clearInterval(interval);
      }
    }, 100); // Dit bepaalt de snelheid van het typen
  });
</script>

<section class="about-me-container">
  <div class="about-me-left">
    <h2>ABOUT ME</h2>
    <p class="intro-1">
      Hi there! My name is {name}, and I'm a frontend developer with love for creating responsive and accessible websites.
    </p>
    <div class="photo-container">
      <img src="/images/photo1.jpg" alt="Photo 1 of {name}" class="profile-photo" />
      <img src="/images/photo2.jpg" alt="Photo 2 of {name}" class="profile-photo" />
    </div>
    <p>
      <strong class="intro-2">
        <span id="typed-text">{typedText}</span>
      </strong>
    </p>
    <hr />
    <div class="about-me-buttons">
      <a href={github} target="_blank" class="button github">GitHub</a>
      <a href={linkedin} target="_blank" class="button linkedin">LinkedIn</a>
      <a href={"mailto:" + email} class="button email">E-mail</a>
    </div>
  </div>
  <div class="about-me-right">
    <h2>WHAT IS A FRONTEND DEVELOPER?</h2>
    <p>
      As a frontend developer, I am passionate about creating user-friendly and visually appealing websites. I use HTML, CSS, and JavaScript to build responsive and interactive interfaces that adapt to various screen sizes. My focus is on optimizing the user experience by developing fast and accessible websites.
    </p>
    <hr />
  </div>
</section>

<style>
  .about-me-container {
    display: flex;
    flex-wrap: wrap;
    padding: 2rem;
    color: white;
  }

  .about-me-left, .about-me-right {
    flex: 1 1 45%;
    margin: 1rem;
  }

  .intro-1 {
    font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    font-size: 1rem;
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

  .about-me-right p {
    font-family: Didot, serif;
    font-family: Courier, monospace;
  }

  .button {
    text-decoration: none;
    padding: 0.5rem 1rem;
    border-radius: 2px;
    color: white;
    background-color: #333;
    transition: background-color 0.3s;
    font-family: Impact, fantasy;
  }

  .button:hover {
    background-color: #555;
  }

  /* Styling for the typing effect text */
  #typed-text {
    display: inline-block;
    font-weight: bold;
  }
</style>
