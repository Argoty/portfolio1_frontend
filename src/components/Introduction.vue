<template>
  <section id="inicio">
    <div class="contenido">
      <header>
        <div class="contenido-header">
          <h1>/JLA/</h1>
          <nav id="nav" class="">
            <ul id="links">
              <li>
                <a
                  href="#inicio"
                  class="seleccionado"
                  @click="seleccionar($event.target)"
                  >HOME</a
                >
              </li>
              <li>
                <a href="#sobremi" @click="seleccionar($event.target)">ABOUT ME</a>
              </li>
              <li>
                <a href="#servicios" @click="seleccionar($event.target)">SERVICES</a>
              </li>
              <li>
                <a href="#portfolio" @click="seleccionar($event.target)">PROJECTS</a>
              </li>
              <li>
                <a href="#contacto" @click="seleccionar($event.target)">CONTACT</a>
              </li>
            </ul>
          </nav>

          <!-- Icono del menu responsive -->
          <div id="icono-nav" @click="responsiveMenu()">
            <i class="fa-solid fa-bars"></i>
          </div>

          <div class="redes">
            <a href="https://www.facebook.com/javier.argoty.3" target="_blank"
              ><i class="fa-brands fa-facebook"></i
            ></a>
            <a href="https://www.instagram.com/argoty__/" target="_blank"
              ><i class="fa-brands fa-instagram-square"></i
            ></a>
          </div>
        </div>
      </header>
      <div class="presentacion">
        <p class="bienvenida">Hi! Welcome to my website</p>
        <h2>I'm <span>Javier Argoty</span>, Web Developer</h2>
        <p class="descripcion">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta,
        </p>
        <a href="#portfolio">Go to the Portfolio</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    seleccionar(link) {
      var opciones = document.querySelectorAll("#links a");
      opciones[0].className = "";
      opciones[1].className = "";
      opciones[2].className = "";
      opciones[3].className = "";
      opciones[4].className = "";
      link.className = "seleccionado";

      //Hacemos desaparecer el menu una vez que se ha seleccionado una opcion
      //en modo responsive
      var x = document.getElementById("nav");
      x.className = "";
    },

    responsiveMenu() {
      var x = document.getElementById("nav");
      if (x.className === "") {
        x.className = "responsive";
      } else {
        x.className = "";
      }
    },
  },
};
</script>

<style>
#inicio {
  background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
    url("@/assets/fondo-inicio.jpg");
  background-size: cover;
  background-position: center center;
  height: 100vh;
}

#inicio .contenido header {
  background-color: rgba(0, 0, 0, 0.8);
  position: fixed;
  width: 100%;
  z-index: 100;
  top: 0;
}

#inicio .contenido header .contenido-header {
  max-width: 1100px;
  margin: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
}

#inicio .contenido header .contenido-header h1 {
  text-align: center;
  color: var(--color);
}

#inicio .contenido header .contenido-header nav ul {
  list-style: none;
  display: flex;
  align-items: center;
}

#inicio .contenido header .contenido-header nav ul li a {
  text-decoration: none;
  color: #fff;
  margin: 0 12px;
  font-weight: 400;
  transition: 0.5s;
}

#inicio .contenido header .contenido-header nav ul li a:hover {
  color: var(--color);
}

#inicio .contenido header .contenido-header .redes a {
  text-decoration: none;
  color: #fff;
  display: inline-block;
  margin-left: 10px;
  transition: 0.5s;
}

#inicio .contenido header .contenido-header .redes a:hover {
  color: var(--color);
}

#inicio .contenido header .contenido-header .seleccionado {
  color: var(--color);
}

#inicio .contenido .presentacion {
  max-width: 1100px;
  height: 100vh;
  margin: auto;
  color: #fff;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

#inicio .contenido .presentacion .bienvenida {
  font-size: 16px;
  margin-bottom: 20px;
  text-transform: uppercase;
  letter-spacing: 5px;
}

#inicio .contenido .presentacion h2 {
  font-size: 55px;
  margin-bottom: 25px;
  text-align: center;
}

#inicio .contenido .presentacion h2 span {
  font-size: 25px;
  color: var(--color);
}

#inicio .contenido .presentacion .descripcion {
  max-width: 700px;
  margin: 25px auto;
  font-size: 18px;
  text-align: center;
}

#inicio .contenido .presentacion a {
  text-decoration: none;
  display: inline-block;
  margin: 25px;
  padding: 20px 25px;
  border: 2px solid #fff;
  border-radius: 50px;
  color: #fff;
  font-weight: bold;
  text-transform: uppercase;
  transition: 0.5s;
}

#inicio .contenido .presentacion a:hover {
  background-color: var(--color);
}

#icono-nav {
  color: #fff;
  display: none;
}
</style>