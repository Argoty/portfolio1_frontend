<template>
  <section id="contacto">
    <h3 class="titulo-seccion">Contact me</h3>
    <div class="contact-row">
      <div class="contact-left">
        <div class="icon-box">
          <div class="icon"><i class="fa-solid fa-envelope"></i></div>

          <div class="info">
            <h4>Email:</h4>
            <p>javierargoty35@gmail.com</p>
          </div>
        </div>

        <div class="icon-box">
          <div class="icon"><i class="fa-solid fa-phone"></i></div>

          <div class="info">
            <h4>Phone:</h4>
            <p>+57 322 2838161</p>
          </div>
        </div>

        <div class="icon-box">
          <div class="icon"><i class="fa-solid fa-location-dot"></i></div>

          <div class="info">
            <h4>Location:</h4>
            <p>Villavicencio, Meta, Colombia</p>
          </div>
        </div>

        <div class="map">
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d127343.4570824251!2d-73.67910116612441!3d4.124925653326942!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8e3e2ddfba283211%3A0x537e40041d7b20c2!2sVillavicencio%2C%20Meta!5e0!3m2!1ses!2sco!4v1680483662332!5m2!1ses!2sco"
            width="100%"
            height="250"
            style="border: 0"
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          ></iframe>
        </div>
      </div>

      <div class="contact-right">
        <form action="">
          <input type="text" name="name" id="name" placeholder="Your Name">
          <input type="email" name="email" id="email" placeholder="Your Email">
          <input type="text" name="subject" id="subject" placeholder="Subject">
          <textarea name="msg" id="msg" rows="9" placeholder="Your Message"> </textarea>
          <input type="submit" value="Send Message">
        </form>
      </div>
    </div>
    <!-- <div class="contenedor-form">
      <form action="">
        <div class="fila mitad">
          <input type="text" placeholder="Full Name *" class="input-mitad" />
          <input type="email" placeholder="Email Address" class="input-mitad" />
        </div>
        <div class="fila">
          <input type="text" placeholder="Subject..." class="input-full" />
        </div>
        <div class="fila">
          <textarea
            name=""
            id=""
            cols="30"
            rows="10"
            placeholder="Message..."
            class="input-full"
          ></textarea>
        </div>

        <input type="submit" value="Send" class="btn-enviar" />
      </form>
    </div> -->
  </section>
</template>

<script>
export default {};
</script>

<style>
#contacto {
  padding: 100px 15px;
  background-color: #f3f3f3;
}

#contacto .titulo-seccion {
  margin-bottom: 20px;
  text-align: center;
  font-size: 22px;
  text-transform: uppercase;
  color: #111135;
  text-decoration: underline;
  text-decoration-color: #d3d3d3;
  text-decoration-thickness: 5px;
}

#contacto .contact-row {
  margin-top: 30px;
  display: flex;
  gap: 20px;
  width: 100%;
}
#contacto .contact-row .contact-left {
  flex-basis: 40%;
  min-width: 40%;
  background-color: white;
  box-shadow: 0 0 20px rgba(0, 0, 0, 20%);
  border-radius: 4px;
  padding: 20px;
}
#contacto .contact-row .contact-left .icon-box {
  display: flex;
  gap: 15px;
  align-items: center;
  margin: 30px 0;
}

#contacto .contact-row .contact-left .icon-box .icon i {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  border: 2px solid var(--color);
  text-align: center;
  line-height: 47px;
  font-size: 20px;
  color: var(--color);
  transition: 0.5s;
}

#contacto .contact-row .contact-left .icon-box:hover .icon i {
  background-color: var(--color);
  color: white;
}
#contacto .contact-row .contact-right {
  flex-basis: 60%;
  min-width: 60%;
  background-color: white;
  box-shadow: 0 0 20px rgba(0, 0, 0, 20%);
  border-radius: 4px;
  padding: 20px;
}

#contacto .contact-row .contact-right form {
  display: flex;
  flex-direction: column;
  gap: 10px;
  margin: 20px 0;
}
#contacto .contact-row .contact-right form input,
#contacto .contact-row .contact-right form textarea {
  display: block;
  width: 100%;
  margin: 10px 0;
  font-size: 15px;
  font-weight: 500;
  padding: 10px 20px;
  border: 2px solid lightgray;
  border-radius: 2px;
  outline: none;
  resize: none;
  transition: 0.5s;
}

#contacto .contact-row .contact-right form input:focus,
#contacto .contact-row .contact-right form textarea:focus {
  border: 2px solid var(--color)
}

#contacto .contact-row .contact-right form input[type=submit] {
  background-color: var(--color);
  color: white;
  border: 2px solid var(--color);
  font-size: 17px;
  font-weight: 400;
  cursor: pointer;
}
/* 

#contacto .contenedor-form {
  max-width: 1100px;
  margin: auto;
}

#contacto .contenedor-form .fila {
  margin-bottom: 15px;
}

#contacto .contenedor-form .mitad {
  display: flex;
  justify-content: space-between;
}

#contacto .contenedor-form input,
#contacto .contenedor-form textarea {
  padding: 20px;
  border-radius: 20px;
  border: none;
  border: 1px solid #919191;
}

#contacto .contenedor-form .mitad input {
  width: 48%;
}

#contacto .contenedor-form .input-full {
  width: 100%;
}



#contacto .btn-enviar {
  display: block;
  font-size: 17px;
  margin: auto;
  cursor: pointer;
  transition: 0.5s;
  padding: 10px 15px !important;
}

#contacto .btn-enviar:hover {
  background-color: var(--color);
  color: #fff;
} */
</style>