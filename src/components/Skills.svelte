<script>
    export let skills = [
      "HTML",
      "CSS",
      "JavaScript",
      "Svelte",
      "SvelteKit",
      "Directus",
      "WordPress",
      "Next.js"
    ];
  </script>
  
  <section class="skills-container">
    <div class="skills-left">
      <h2>MY SKILLS</h2>
      <ul class="skills-list">
        {#each skills as skill}
          <li>{skill}</li>
        {/each}
      </ul>
    </div>
    <div class="skills-right">
      <h2>WHY THESE TECHNOLOGIES?</h2>
      <p>
        I use HTML, CSS, and JavaScript as the core building blocks for creating web applications. 
        Svelte and SvelteKit help me create highly efficient and interactive user interfaces. 
        Directus and WordPress allow me to manage content effectively.
      </p>
    </div>
  </section>
  
  <style>
    .skills-container {
      display: flex;
      flex-wrap: wrap;
      padding: 2rem;
      color: white;
    }
  
    .skills-left,
    .skills-right {
      flex: 1 1 45%;
      margin: 1rem;
    }
  
    .skills-list {
      list-style: none;
      padding: 0;
      font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
      font-size: 1rem;
      line-height: 1.8;
    }
  
    .skills-list li {
      margin: 0.5rem 0;
      background: #222;
      padding: 0.5rem 1rem;
      border-radius: 4px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      font-family: Courier, monospace;
    }
  
    .skills-right p {
      font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
      font-size: 1rem;
    }
  
    h2 {
      font-size: 1.5rem;
      color: #ff6347;
    }
  
    /* hr {
      border: none;
      height: 1px;
      background: #555;
      margin: 1.5rem 0;
    } */
  </style>