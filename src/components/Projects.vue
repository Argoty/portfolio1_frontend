<template>
  <section id="portfolio">
    <h3 class="titulo-seccion">My projects</h3>
    <div class="fila">
      <div class="proyecto">
        <div class="overlay"></div>
        <img :src="require('@/assets/proyecto1.jpg')" alt="" />
        <div class="info">
          <h4>Descripcion Proyecto</h4>
          <p>Diseño Web</p>
        </div>
      </div>
      <div class="proyecto">
        <div class="overlay"></div>
        <img :src="require('@/assets/proyecto2.jpg')" alt="" />
        <div class="info">
          <h4>Descripcion Proyecto</h4>
          <p>Diseño Web</p>
        </div>
      </div>
      <div class="proyecto">
        <div class="overlay"></div>
        <img :src="require('@/assets/proyecto3.jpg')" alt="" />
        <div class="info">
          <h4>Descripcion Proyecto</h4>
          <p>Diseño Web</p>
        </div>
      </div>
    </div>
    <div class="fila">
      <div class="proyecto">
        <div class="overlay"></div>
        <img :src="require('@/assets/proyecto4.jpg')" alt="" />
        <div class="info">
          <h4>Descripcion Proyecto</h4>
          <p>Diseño Web</p>
        </div>
      </div>
      <div class="proyecto">
        <div class="overlay"></div>
        <img :src="require('@/assets/proyecto5.jpg')" alt="" />
        <div class="info">
          <h4>Descripcion Proyecto</h4>
          <p>Diseño Web</p>
        </div>
      </div>
      <div class="proyecto">
        <div class="overlay"></div>
        <img :src="require('@/assets/proyecto6.jpg')" alt="" />
        <div class="info">
          <h4>Descripcion Proyecto</h4>
          <p>Diseño Web</p>
        </div>
      </div>
    </div>
    <div class="fila">
      <div class="proyecto">
        <div class="overlay"></div>
        <img :src="require('@/assets/proyecto7.jpg')" alt="" />
        <div class="info">
          <h4>Descripcion Proyecto</h4>
          <p>Diseño Web</p>
        </div>
      </div>
      <div class="proyecto">
        <div class="overlay"></div>
        <img :src="require('@/assets/proyecto8.jpg')" alt="" />
        <div class="info">
          <h4>Descripcion Proyecto</h4>
          <p>Diseño Web</p>
        </div>
      </div>
      <div class="proyecto">
        <div class="overlay"></div>
        <img :src="require('@/assets/proyecto9.jpg')" alt="" />
        <div class="info">
          <h4>Descripcion Proyecto</h4>
          <p>Diseño Web</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
#portfolio {
  max-width: 1100px;
  padding: 100px 0;
  margin: auto;
}

#portfolio .titulo-seccion {
  text-align: center;
  font-size: 22px;
  text-transform: uppercase;
  color: #111135;
  text-decoration: underline;
  text-decoration-color: #d3d3d3;
  text-decoration-thickness: 5px;
}

#portfolio .fila {
  display: flex;
  justify-content: space-between;
  margin: 30px 0;
}

#portfolio .fila .proyecto {
  max-width: 450px;
  border: 1px solid #000;
  margin: 0 10px;
  position: relative;
  overflow: hidden;
}

#portfolio .fila .proyecto img {
  width: 100%;
  height: 100%;
  filter: grayscale(1);
  object-fit: cover;
  transition: 0.5s;
}

#portfolio .fila .proyecto:hover img {
  filter: grayscale(0);
}

#portfolio .fila .proyecto .info {
  position: absolute;
  left: 0px;
  background-color: rgba(0, 0, 0, 0.8);
  color: var(--color);
  width: 100%;
  padding: 10px;
  opacity: 0;
  bottom: -40px;
  transition: 0.5s;
}

#portfolio .fila .proyecto:hover .info {
  opacity: 1;
  bottom: 0;
}
</style>