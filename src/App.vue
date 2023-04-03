<template>
  <Introduction />
  <AboutMe />
  <Services />
  <Skills />
  <Projects />
  <Contact />
  <Footer />
</template>

<script>
import Introduction from "./components/Introduction.vue";
import AboutMe from "./components/AboutMe.vue";
import Services from "./components/Services.vue";
import Skills from "./components/Skills.vue";
import Projects from "./components/Projects.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Introduction,
    AboutMe,
    Services,
    Skills,
    Projects,
    Contact,
    Footer,
  },
};
</script>

<style>
:root {
  --color: #ff4848;
}

@import url('https://fonts.googleapis.com/css2?family=Rubik&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Rubik', sans-serif;
  
}

html {
  scroll-behavior: smooth;
}

@media screen and (max-width: 800px) {
  .redes {
    display: none;
  }
  nav {
    display: none;
  }
  nav.responsive {
    display: block;
    background-color: rgba(0, 0, 0, 0.8);
    width: 100%;
    position: absolute;
    top: 48px;
    left: 0;
    padding: 10px 0;
  }
  nav.responsive ul {
    display: block !important;
    text-align: center;
  }
  nav.responsive ul li {
    margin: 5px 0;
  }
  #icono-nav {
    display: block;
  }
  #inicio .contenido .presentacion h2 {
    font-size: 40px;
  }
  /* seccion SOBRE MI */
  #sobremi {
    padding: 50px 0;
    display: block;
  }
  #sobremi .contenedor-foto {
    max-width: 200px;
    margin: auto;
  }
  #sobremi .contenedor-foto img {
    padding: 8px;
  }
  #sobremi .sobremi .titulo-seccion {
    text-align: center;
  }
  #sobremi .sobremi h2 {
    font-size: 25px;
    text-align: center;
  }
  /* seccion MIS SERVICIOS */
  #servicios {
    padding: 50px 15px;
  }
  #servicios .fila {
    display: block;
  }
  #servicios .fila .servicio {
    margin: 10px auto;
  }
  /* seccion HABLIDADES MI */
  .contenedor-skills {
    padding: 50px 20px;
  }
  .contenedor-skills .skills-row {
    grid-template-columns: repeat(2, 1fr);
  }
  /* seccion PORTFOLIO */
  #portfolio {
    padding: 50px 0;
  }
  #portfolio .fila {
    display: block;
  }
  #portfolio .fila .proyecto {
    margin: 10px auto;
  }
  /* seccion CONTACTO */
  #contacto {
    padding: 50px 15px;
  }
  #contacto .contact-row {
    flex-direction: column;
    gap: 10px
  }
  
}
</style>
