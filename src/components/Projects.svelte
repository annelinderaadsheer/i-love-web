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
    // { 
    //   title: "Project 3", 
    //   link: "https://github.com/annelinderaadsheer", 
    //   image: "/images/project3-logo.png" 
    // },
    // { 
    //   title: "Project 4", 
    //   link: "https://github.com/annelinderaadsheer", 
    //   image: "/images/project4-logo.png" 
    // },
  ];
</script>

<section class="my-projects-container">
  <h2>SOME OF MY PROJECTS</h2>
  <div class="project-grid">
    {#each projects as project}
      <a href={project.link} class="project-item">
        <!-- Alleen het logo wordt weergegeven, de titel is verwijderd -->
        <img src={project.image} alt={project.link} class="project-logo" />
      </a>
    {/each}
  </div>
</section>

<style>
  .my-projects-container {
    padding: 2rem;
    background-color: var(--color-light-pink);
    color: var(--color-dark-pink);
  }

  .my-projects-container h2 {
    text-align: center;
  }

  .project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    gap: 1rem;
  }

  .project-item {
    text-align: center;
    padding: 1.5rem;
    border-radius: 4px;
    /* text-decoration: none; */
    /* transition: background-color 0.3s; */
    /* background-color: white; */
  }

  .project-item:hover {
    background-color: var(--color-orange);
  }

  .project-logo {
    max-width: 100%;
    margin-bottom: 1rem;
    margin-top: 1rem;
  }
</style>