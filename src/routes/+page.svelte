<script>
    import Header from '../components/Header.svelte';
    import AboutMe from '../components/AboutMe.svelte';
    import Projects from '../components/Projects.svelte';
    import Skills from '../components/Skills.svelte'
    // import WeLoveWeb from '../components/WeLoveWeb.svelte';
  </script>
  
  <main>
    <Header />
    <AboutMe />
    <Projects />
    <Skills />
    <!-- <WeLoveWeb /> -->
  </main>
  
  <style>
    main {
      font-family: 'Arial', sans-serif;
      color: white;
      background-color: #000;
      margin: 0;
      padding: 0;
      min-height: 100vh;
    }
  </style>
