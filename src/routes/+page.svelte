<script>


</script>

<main>
    <h1>MY PORTFOLIO</h1>
    <section class="about-me-container">
        <div class="about-me-left">
            <h2>ABOUT ME</h2>
            <p class="intro-1">Hi there! My name is Annelinde, and I'm a frontend developer with love for creating responsive and accessible websites.</p>
            <p><strong class="intro-2"><span id="typed-text"></span>LET'S CREATE SOMETHING TOGETHER.</strong><p>
            <hr> 
            <div class="about-me-buttons">
                <a href="https://github.com/annelinderaadsheer" target="_blank" class="button github">GitHub</a>
                <a href="https://www.linkedin.com/in/annelinde-raadsheer-b38375194/" target="_blank" class="button linkedin">LinkedIn</a>
                <a href="mailto:anne_linde@live.nl" class="button email">E-mail</a>
            </div>
        </div>
        <div class="about-me-right">
            <h2>WHAT IS A FRONTEND DEVELOPER?</h2>
            <p>As a frontend developer, I am passionate about creating user-friendly and visually appealing websites. I use HTML, CSS, and JavaScript to build responsive and interactive interfaces that adapt to various screen sizes. My focus is on optimizing the user experience by developing fast and accessible websites.</p>
            <hr> 
        </div>
    </section>

    <section class="my-projects-container">
        <h2>SOME OF MY PROJECTS</h2>
        <div class="project-grid">
            <a href="https://github.com/annelinderaadsheer" class="project-item-1">
                <!-- <img src="" alt="Project 1"> -->
                <p>Project 1</p>
            </a>
            <a href="https://github.com/annelinderaadsheer" class="project-item-2">
                <!-- <img src="" alt="Project 2"> -->
                <p>Project 2</p>
            </a>
            <a href="https://github.com/annelinderaadsheer" class="project-item-3">
                <!-- <img src="" alt="Project 3"> -->
                <p>Project 3</p>
            </a>
            <a href="https://github.com/annelinderaadsheer" class="project-item-4">
                <!-- <img src="" alt="Project 4"> -->
                <p>Project 4</p>
            </a>
            <a href="https://github.com/annelinderaadsheer" class="project-item-5">
                <!-- <img src="" alt="Project 5"> -->
                <p>Project 5</p>
            </a>
            <a href="https://github.com/annelinderaadsheer" class="project-item-6">
                <!-- <img src="" alt="Project 6"> -->
                <p>Project 6</p>
            </a>
        </div>
    </section>    
    
</main>

<style lang="scss">

:root {
    --primary-color: #2C2C2C; /* Donkergrijs */
    --secondary-color: #FDFDFD; /* Wit */
    --accent-color: #EBE9E3; /* Creme */
    --neutral-color: #D9D5C9; /* Beige */
}

main {
    font-family: Arial, sans-serif;
    background-color: var(--neutral-color);
    padding: 35px;
}

h1 {
    color: var(--primary-color);
}

a {
    color: #007BFF;
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
}

/* ABOUT ME */

.about-me-container {
    background: var(--primary-color);
    border: 1px solid #ddd;
    padding: 15px;
    margin-bottom: 20px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    display: flex;
    justify-content: space-between; 
    min-height: 200px;
}

.about-me-left {
    color: var(--secondary-color);
    width: 25%;
    margin-left: 25px;
}

.intro-1 {
    font-family: Georgia, 'Times New Roman', Times, serif;
    font-size: 18px;
}

.intro-2 {
    border-right: 2px solid var(--secondary-color); 
    overflow: hidden; 
    width: 0;
    animation: typing 5s steps(30, end), blink-caret 0.75s step-end infinite; 
    color: var(--secondary-color);
    font-size: 16px;
}

@keyframes typing {
    from { width: 0; }
    to { width: 100%; }
}

@keyframes blink-caret {
    50% { border-color: transparent; } /* Knipperend effect */
}

.about-me-right {
    color: var(--secondary-color);
    width: 35%; 
    margin-right: 25px;
    margin-top: 15px;
}

.about-me-right h2 {
font-size: 16px;
}

.about-me-right p {
    font-family: Georgia, 'Times New Roman', Times, serif;
    font-size: 18px;
}

.about-me-buttons {
    display: flex;
    flex-direction: column;   
    margin-top: 25px; 
}

.button {
    padding: 10px 15px;
    text-decoration: none; 
    color: var(--secondary-color);
    border-radius: 5px;
    font-weight: bold;
    width: 100%; /* Knoppen vullen de breedte van de container */
    max-width: 200px; /* Maximale breedte van de knoppen */
    text-align: center; 
    margin-bottom: 10px;
}

.github {
    background-color: transparent;
    border: 1px solid white;
}

.linkedin {
    background-color: transparent;
    border: 1px solid white;
}

.email {
    background-color: transparent;
    border: 1px solid white;
}

/* ABOUT ME MEDIA QUERIES */

@media (max-width: 768px) {
    .about-me-container {
        flex-direction: column; /* Zorgt ervoor dat de secties onder elkaar komen op kleinere schermen */
    }

    .about-me-left, .about-me-right {
        width: 100%;
        margin-left: 0;
    }
}

/* MY PROJECTS */

.my-projects-container {
    background: var(--primary-color);
    border: 1px solid #ddd;
    padding: 15px;
    margin-bottom: 20px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    text-align: center;
    min-height: 250px;
}

.my-projects-container h2 {
    color: var(--accent-color);
}

.project-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px; /* Ruimte tussen de blokken */
    justify-items: center; /* Horizontaal centreren */
    align-items: center; /* Verticaal centreren */
    margin-left: 25px;
    margin-right: 25px;
}

.project-item-1 {
    background-color: transparent;
    border: 1px solid white;
    width: 250px;
    height: 250px;
}

.project-item-2 {
    background-color: transparent;
    border: 1px solid white;
    width: 250px;
    height: 250px;
}

.project-item-3 {
    background-color: transparent;
    border: 1px solid white;
    width: 250px;
    height: 250px;
}

.project-item-4 {
    background-color: transparent;
    border: 1px solid white;
    width: 250px;
    height: 250px;
}

.project-item-5 {
    background-color: transparent;
    border: 1px solid white;
    width: 250px;
    height: 250px;
}

.project-item-6 {
    background-color: transparent;
    border: 1px solid white;
    width: 250px;
    height: 250px;
}

</style>