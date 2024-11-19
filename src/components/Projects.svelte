<script>
    export let projects = [
      { title: "Project 1", link: "https://github.com/annelinderaadsheer" },
      { title: "Project 2", link: "https://github.com/annelinderaadsheer" },
      { title: "Project 3", link: "https://github.com/annelinderaadsheer" },
      { title: "Project 4", link: "https://github.com/annelinderaadsheer" },
      { title: "Project 5", link: "https://github.com/annelinderaadsheer" },
      { title: "Project 6", link: "https://github.com/annelinderaadsheer" },
    ];
  </script>
  
  <section class="my-projects-container">
    <h2>SOME OF MY PROJECTS</h2>
    <div class="project-grid">
      {#each projects as project}
        <a href={project.link} class="project-item">
          <p>{project.title}</p>
        </a>
      {/each}
    </div>
  </section>
  
  <style>
    .my-projects-container {
      padding: 2rem;
      /* background-color: #111; */
      color: white;
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
      padding: 1rem;
      border: 1px solid #333;
      border-radius: 5px;
      text-decoration: none;
      color: white;
      transition: background-color 0.3s;
    }
  
    .project-item:hover {
      background-color: #333;
    }
  </style>
  