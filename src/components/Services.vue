<template>
  <section id="servicios">
    <h3 class="titulo-seccion">My Services</h3>
    <div class="fila">
      <div class="servicio">
        <span class="icono"> <i class="fa-solid fa-code"></i></span>
        <h4>Diseño de Sitios Web</h4>
        <hr />
        <ul class="servicios-tag">
          <li>Web</li>
          <li>Graphic</li>
          <li>SEO</li>
        </ul>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit
          voluptatibus rem illum sunt, asperiores!
        </p>
      </div>
      <div class="servicio">
        <span class="icono"><i class="fa-solid fa-file-code"></i></span>
        <h4>Porgramación PHP</h4>
        <hr />
        <ul class="servicios-tag">
          <li>Web</li>
          <li>Graphic</li>
          <li>SEO</li>
        </ul>
        <p>
          I have been providing web design services with great success for 9
          years. The client is very happy
        </p>
      </div>
      <div class="servicio">
        <span class="icono"><i class="fa-solid fa-arrow-trend-up"></i></span>
        <h4>Posicionamiento SEO</h4>
        <hr />
        <ul class="servicios-tag">
          <li>Web</li>
          <li>Graphic</li>
          <li>SEO</li>
        </ul>
        <p>
          I have been providing web design services with great success for 9
          years. The client is very happy
        </p>
      </div>
    </div>
    <div class="fila">
      <div class="servicio">
        <span class="icono"><i class="fa-solid fa-database"></i></span>
        <h4>Alojamiento de Sitios</h4>
        <hr />
        <ul class="servicios-tag">
          <li>Web</li>
          <li>Graphic</li>
          <li>SEO</li>
        </ul>
        <p>
          I have been providing web design services with great success for 9
          years. The client is very happy
        </p>
      </div>
      <div class="servicio">
        <span class="icono"><i class="fa-solid fa-palette"></i></span>
        <h4>Diseñador Gráfico</h4>
        <hr />
        <ul class="servicios-tag">
          <li>Web</li>
          <li>Graphic</li>
          <li>SEO</li>
        </ul>
        <p>
          I have been providing web design services with great success for 9
          years. The client is very happy
        </p>
      </div>
      <div class="servicio">
        <span class="icono"
          ><i class="fa-solid fa-person-circle-question"></i
        ></span>
        <h4>Consultor Externo</h4>
        <hr />
        <ul class="servicios-tag">
          <li>Web</li>
          <li>Graphic</li>
          <li>SEO</li>
        </ul>
        <p>
          I have been providing web design services with great success for 9
          years. The client is very happy
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
#servicios {
  padding: 100px 15px;
  text-align: center;
  background-color: #f3f3f3;
}

#servicios .titulo-seccion {
  text-align: center;
  font-size: 22px;
  text-transform: uppercase;
  color: #111135;
  text-decoration: underline;
  text-decoration-color: #d3d3d3;
  text-decoration-thickness: 5px;
}

#servicios .fila {
  display: flex;
  justify-content: space-between;
  max-width: 1150px;
  margin: 30px auto;
}

#servicios .fila .servicio {
  max-width: 350px;
  background-color: #fff;
  padding: 30px;
  margin: 0 5px;
  border-radius: 5px;
  transition: 0.5s;
}

#servicios .fila .servicio:hover {
  box-shadow: 5px 5px 10px #565656, -5px -5px 10px #8a8a8a;
}

#servicios .fila .servicio .icono {
  display: inline-block;
  width: 60px;
  height: 60px;
  border-radius: 50%;
  background-color: #d3d3d3;
  padding: 20px;
  margin-bottom: 25px;
}

#servicios .fila .servicio h4 {
  font-size: 22px;
  margin-bottom: 25px;
}

#servicios .fila .servicio hr {
  width: 30%;
  margin: auto;
  color: #000;
  margin-bottom: 25px;
}

#servicios .fila .servicio ul {
  list-style: none;
  display: flex;
  justify-content: space-around;
  margin-bottom: 10px;
}

#servicios .fila .servicio p {
  font-size: 14px;
  line-height: 22px;
}
</style>