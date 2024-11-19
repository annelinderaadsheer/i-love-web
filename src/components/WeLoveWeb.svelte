<script>
    export let items = [
      "We love web 1",
      "We love web 2",
      "We love web 3",
      "We love web 4",
      "We love web 5",
      "We love web 6",
    ];
  </script>
  
  <section class="we-love-web-container">
    <div class="we-love-web-left">
      <h2>WE LOVE WEBS</h2>
      <hr />
      <div class="we-love-web">
        {#each items as item, i}
          <a href="#" class="we-love-web-item">
            <p>{item}</p>
          </a>
        {/each}
      </div>
    </div>
    <div class="learning-journal-right">
      <h2>MY LEARNING JOURNAL</h2>
      <hr />
    </div>
  </section>
  
  <style>
    .we-love-web-container {
      display: flex;
      padding: 2rem;
      /* background-color: #222; */
      color: white;
    }
  
    .we-love-web-left, .learning-journal-right {
      flex: 1 1 50%;
      margin: 1rem;
    }
  
    .we-love-web {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
    }
  
    .we-love-web-item {
      text-decoration: none;
      color: white;
      background-color: #333;
      padding: 0.5rem 1rem;
      border-radius: 5px;
    }
  
    .we-love-web-item:hover {
      background-color: #555;
    }
  </style>