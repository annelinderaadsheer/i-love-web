<script>
  export let skills = [
    { name: "HTML", level: 100 },
    { name: "CSS", level: 100 },
    { name: "JavaScript", level: 50 },
    { name: "Svelte", level: 100 },
    { name: "SvelteKit", level: 100 },
    { name: "Directus", level: 50 },
    { name: "WordPress", level: 50 },
    { name: "Next.js", level: 30 }
  ];
</script>

<section class="skills-container">
  <section class="skills-left">
    <h2>MY SKILLS</h2>
    <ul class="skills-list">
      {#each skills as skill}
        <li class="skill-item" style="--skill-level: {skill.level}%">
          <span>{skill.name}</span>
        </li>
      {/each}
    </ul>
  </section>
  <section class="skills-right">
    <h2>WHY THESE SKILLS?</h2>
    <p>
      I use HTML, CSS, and JavaScript as the core building blocks for creating web applications. 
      Svelte and SvelteKit help me create highly efficient and interactive user interfaces. 
      Directus and WordPress allow me to manage content effectively.
    </p>
  </section>
</section>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Abril+Fatface&family=Montserrat:wght@400;700&display=swap');

  .skills-container {
    display: flex;
    flex-wrap: wrap;
    padding: 2rem;
    color: var(--color-dark-pink);
    background-color: var(--color-light-pink);
    font-family: 'Montserrat', sans-serif;
  }

  .skills-left,
  .skills-right {
    flex: 1 1 45%;
    margin: 1rem;
  }

  .skills-list {
    list-style: none;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
    font-size: 1rem;
    line-height: 1.8;
  }

  .skills-list li {
    margin: 0.5rem 0;
    background-color: var(--color-white);
    padding: 0.5rem 1rem;
    border-radius: 4px;
    border: 2px solid var(--color-dark-pink);
    box-shadow: 0 3px 5px rgba(0, 0, 0, 0.15);
    font-family: 'Montserrat', sans-serif;
    letter-spacing: 1px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;
  }

  .skills-list li::after {
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 4px;
    background-color: var(--color-orange);
    width: 0%;
    border-radius: 4px;
    transition: width 0.5s ease;
  }

  .skills-list li:hover::after {
    width: var(--skill-level); 
  }

  .skills-list span {
    font-weight: bold;
    color: var(--color-red);
  }

  .skills-right p {
    font-family: 'Montserrat', sans-serif;
    font-size: 1.2rem;
    line-height: 1.6;
  }

  h2 {
    font-family: 'Abril Fatface', serif;
    font-size: 2rem;
    color: var(--color-red);
  }

  /* Media Queries */
  @media (min-width: 320px) {
    .skills-container {
      font-size: 1rem;
    }

    .skills-left,
    .skills-right {
      flex: 1 1 100%;
    }

    .skills-list {
      font-size: 0.9rem;
    }

    .skills-right p {
      font-size: 1rem;
    }
  }

  @media (min-width: 480px) {
    .skills-container {
      font-size: 1.2rem;
    }

    .skills-left,
    .skills-right {
      flex: 1 1 45%;
    }

    .skills-list {
      font-size: 1rem;
    }

    .skills-right p {
      font-size: 1.1rem;
    }
  }

  @media (min-width: 768px) {
    .skills-container {
      font-size: 1.4rem;
    }

    .skills-left,
    .skills-right {
      flex: 1 1 45%;
    }

    .skills-list {
      font-size: 1.1rem;
    }

    .skills-right p {
      font-size: 1.2rem;
    }
  }

  @media (min-width: 1024px) {
    .skills-container {
      font-size: 1.6rem;
    }

    .skills-left,
    .skills-right {
      flex: 1 1 45%;
    }

    .skills-list {
      font-size: 1.2rem;
    }

    .skills-right p {
      font-size: 1.3rem;
    }
  }

  @media (min-width: 1280px) {
    .skills-container {
      font-size: 1.8rem;
    }

    .skills-left,
    .skills-right {
      flex: 1 1 45%;
    }

    .skills-list {
      font-size: 1.3rem;
    }

    .skills-right p {
      font-size: 1.4rem;
    }
  }

  @media (min-width: 1440px) {
    .skills-container {
      font-size: 2rem;
    }

    .skills-left,
    .skills-right {
      flex: 1 1 45%;
    }

    .skills-list {
      font-size: 1.4rem;
    }

    .skills-right p {
      font-size: 1.5rem;
    }
  }

  @media (min-width: 1920px) {
    .skills-container {
      font-size: 2.2rem;
    }

    .skills-left,
    .skills-right {
      flex: 1 1 45%;
    }

    .skills-list {
      font-size: 1.5rem;
    }

    .skills-right p {
      font-size: 1.6rem;
    }
  }
</style>
