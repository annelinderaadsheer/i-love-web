<script>
  export let projects = [
    { 
      title: "Redpers", 
      link: "https://github.com/annelinderaadsheer/lose-your-head-the-client-case", 
      image: "/images/Redpers-logo.webp"
    },
    { 
      title: "Oba", 
      link: "https://github.com/annelinderaadsheer/oba", 
      image: "/images/Oba-logo.webp" 
    },
  ];
</script>

<section class="my-projects-container">
  <h2>SOME OF MY PROJECTS</h2>
  <div class="project-grid">
    {#each projects as project}
      <a href={project.link} class="project-item button">
        <img src={project.image} alt={project.link} class="project-logo" />
      </a>
    {/each}
  </div>
</section>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Abril+Fatface&family=Montserrat:wght@400;700&display=swap');

  .my-projects-container {
    padding: 2rem;
    background-color: var(--color-light-pink);
    color: var(--color-red);
    font-family: 'Abril Fatface', serif;
    font-size: 1.5rem;
    text-align: center;
    margin-bottom: 0; 
  }

  .my-projects-container h2 {
    margin-bottom: 1rem; 
  }

  .project-grid {
    display: flex;
    justify-content: center;
    gap: 0.5rem;
    margin: 0 auto; 
    padding: 0; 
    flex-wrap: nowrap; 
  }

  .button {
    border-radius: 4px;
    color: var(--color-red);
    background-color: var(--color-white);
    border: 2px solid var(--color-dark-pink);
    transition: background-color 0.3s, box-shadow 0.3s, transform 0.3s;
    font-family: 'Montserrat', sans-serif;
    box-shadow: 0 3px 5px rgba(0, 0, 0, 0.15);
    display: flex;
    justify-content: center;
    align-items: center;
    aspect-ratio: 1 / 1;
    height: 120px;
    width: 120px;
  }

  .button:hover {
    background-color: var(--color-grey);
    color: var(--color-red);
    box-shadow: 0 5px 10px rgba(0, 0, 0, 0.3);
    transform: translateY(-2px) scale(1.01);
  }

  .project-item {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .project-logo {
    max-width: 80%;
    max-height: 80%;
  }

  /* Media Queries */
  @media (min-width: 320px) {
    .my-projects-container {
      font-size: 1.2rem;
    }
    .project-grid {
      gap: 0.25rem;
    }
    .button {
      height: 120px;
      width: 120px;
    }
  }

  @media (min-width: 480px) {
    .my-projects-container {
      font-size: 1.3rem;
    }
    .project-grid {
      gap: 0.5rem;
    }
    .button {
      height: 130px;
      width: 130px;
    }
  }

  @media (min-width: 768px) {
    .my-projects-container {
      font-size: 1.4rem; 
    }
    .project-grid {
      gap: 1rem;
    }
    .button {
      height: 140px;
      width: 140px;
    }
  }

  @media (min-width: 1024px) {
    .my-projects-container {
      font-size: 1.6rem; 
    }
    .project-grid {
      gap: 1rem;
    }
    .button {
      height: 150px;
      width: 150px;
    }
  }

  @media (min-width: 1280px) {
    .my-projects-container {
      font-size: 1.8rem;
    }
    .project-grid {
      gap: 1rem;
    }
    .button {
      height: 160px;
      width: 160px;
    }
  }

  @media (min-width: 1440px) {
    .my-projects-container {
      font-size: 2rem;
    }
    .project-grid {
      gap: 1rem;
    }
    .button {
      height: 140px;
      width: 140px;
    }
  }

  @media (min-width: 1920px) {
    .my-projects-container {
      font-size: 2.2rem;
    }
    .project-grid {
      gap: 1rem;
    }
    .button {
      height: 120px;
      width: 120px;
    }
  }
</style>

