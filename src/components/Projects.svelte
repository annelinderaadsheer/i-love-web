<section class="my-projects-container">
  <h2>SOME OF MY PROJECTS</h2>

  <!-- Carousel -->
  <div id="carousel">
    <!-- Radio buttons als navigatie -->
    <input type="radio" id="slide1" name="carousel" checked>
    <input type="radio" id="slide2" name="carousel">
    
    <!-- Carousel items -->
    <div class="inner">
      <a href="https://github.com/annelinderaadsheer/lose-your-head-the-client-case" class="project-item button slide">
        <img src="/images/Redpers-logo.webp" alt="Redpers" class="project-logo">
      </a>
      <a href="https://github.com/annelinderaadsheer/oba" class="project-item button slide">
        <img src="/images/Oba-logo.webp" alt="Oba" class="project-logo">
      </a>
    </div>

    <!-- Bullets -->
    <div id="bullets">
      <label for="slide1"></label>
      <label for="slide2"></label>
    </div>
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

  /* Carousel */
  #carousel {
    position: relative;
    overflow: hidden;
    width: 100%;
    max-width: 800px;
    margin: 0 auto;
  }

  /* Verberg standaard radio buttons */
  #carousel input[type="radio"] {
    display: none;
}

  .inner {
    display: flex;
    transition: transform 0.5s ease;
  }

  .slide {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 300px;
    flex: 0 0 100%;
  }

  .project-logo {
    max-width: 80%;
    max-height: 80%;
  }

  /* Bullets styling */
  #bullets {
    display: flex;
    justify-content: center;
    margin-top: 1rem;
  }

  #bullets label {
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background-color: #ccc;
    margin: 0 5px;
    display: inline-block;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }

  #bullets input[type="radio"]:checked + label {
    background-color: #444;
  }

  #bullets label:hover {
    background-color: #999;
  }

  /* Verschuift de carousel naar links of rechts afhankelijk van de geselecteerde radio-button */
  input[type="radio"]:nth-child(1):checked ~ .inner {
    transform: translateX(0%);
  }
  input[type="radio"]:nth-child(2):checked ~ .inner {
    transform: translateX(-100%);
  }
  
  input[type="radio"]:nth-child(3):checked ~ .inner {
    transform: translateX(-200%);
  }
</style>