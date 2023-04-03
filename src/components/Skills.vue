<template>
  <div class="contenedor-skills" id="skills">
    <h3>Skills</h3>
    <div class="skills-row">
      <div class="skill-box">
        <i class="fa-brands fa-html5"></i>
      <strong>Html</strong>
      <p>Intermediate</p>
    </div>

    <div class="skill-box">
      <i class="fa-brands fa-css3"></i>
      <strong>Css</strong>
      <p>Basic</p>
    </div>

    <div class="skill-box">
      <i class="fa-brands fa-js"></i>
      <strong>Javascript</strong>
      <p>Intermediate</p>
    </div>
    <div class="skill-box">
      <i class="fa-brands fa-python"></i>
      <strong>Python</strong>
      <p>Basic</p>
    </div>
    <div class="skill-box">
      <i class="fa-brands fa-vuejs"></i>
      <strong>Vue js</strong>
      <p>Intermediate</p>
    </div>
    <div class="skill-box">
      <i class="fa-solid fa-bolt"></i>
      <strong>FastAPI</strong>
      <p>Basic</p>
    </div>
    <div class="skill-box">
      <i class="fa-brands fa-git-alt"></i>
      <strong>Git</strong>
      <p>Basic</p>
    </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.contenedor-skills {
  background: linear-gradient(#e14747cc, rgba(33, 16, 16, 0.8)),
    url("@/assets/fondo-skills.jpg");
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: cover;
  color: #fff;
  background-position: center center;
  padding: 100px 0;
  text-align: center;
}

.contenedor-skills h3{
  font-size: 22px;
  text-transform: uppercase;
  text-decoration: underline;
  text-decoration-color: #d3d3d3;
  text-decoration-thickness: 5px;
}

.contenedor-skills .skills-row {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 30px;
  margin-top: 50px;
}

.contenedor-skills .skills-row .skill-box i{
  font-size: 40px;
}

.contenedor-skills .skills-row .skill-box strong{
  font-size: 25px;
  margin-left: 5px;
  font-weight: 600;
}

.contenedor-skills .skills-row .skill-box p{
  font-weight: 500;
  font-size: 16px;
}
</style>