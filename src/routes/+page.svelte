<script>
    import Header from '../components/Header.svelte';
    import AboutMe from '../components/AboutMe.svelte';
    import Projects from '../components/Projects.svelte';
    import Skills from '../components/Skills.svelte';
    import Footer from '../components/Footer.svelte'
  </script>

<link rel="stylesheet" href="/styles/variables.css" />
  
  <main>
    <Header />
    <AboutMe />
    <Skills />
    <Projects />
    <Footer />
  </main>
  
  <style>
    main {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      min-height: 100vh;
    }
  </style>
