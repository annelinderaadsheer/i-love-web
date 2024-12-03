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
  }

  .my-projects-container h2 {
    text-align: center;
  }

  .project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    gap: 1rem;
  }

  .button {
    border-radius: 4px;
    color: var(--color-red);
    background-color: var(--color-white);
    border: 2px solid var(--color-dark-pink);
    transition: background-color 0.3s, box-shadow 0.3s, transform 0.3s;
    font-family: 'Montserrat', sans-serif;
    box-shadow: 0 3px 5px rgba(0, 0, 0, 0.15);
    padding: 1rem;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 150px;
  }

  .button:hover {
    background-color: var(--color-grey);
    color: var(--color-red);
    box-shadow: 0 5px 10px rgba(0, 0, 0, 0.3);
    transform: translateY(-5px);
  }

  .project-item {
    padding: 1rem;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 150px;
  }

  .project-logo {
    max-width: 50%;
  }

  /* Media Queries */
  @media (min-width: 300px) {
    .my-projects-container {
      font-size: 1.4rem;
    }
    .project-grid {
      grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
    }
    .project-logo {
      max-width: 100%;
    }
    .button {
      height: 120px;
    }
  }

  @media (min-width: 500px) {
    .my-projects-container {
      font-size: 1.4rem;
    }
    .project-grid {
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    }
    .project-logo {
      max-width: 50%;
    }
    .button {
      height: 130px;
    }
  }

  @media (min-width: 700px) {
    .my-projects-container {
      font-size: 1.5rem; 
    }
    .project-grid {
      grid-template-columns: repeat(auto-fit, minmax(50px, 1fr));
    }
    .project-logo {
      max-width: 50%;
    }
    .button {
      height: 140px;
    }
  }

  @media (min-width: 1000px) {
    .my-projects-container {
      font-size: 1.6rem; 
    }
    .project-grid {
      grid-template-columns: repeat(auto-fit, minmax(50px, 1fr));
    }
    .project-logo {
      max-width: 50%;
    }
    .button {
      height: 150px;
    }
  }
</style>