<template>
  <footer>
    <p>All rights reserved - {{ new Date().getFullYear() }}</p>
    <div class="redes">
      <a href="https://www.facebook.com/javier.argoty.3" target="_blank"><i class="fa-brands fa-facebook"></i></a>
      <a href="https://www.instagram.com/argoty__/" target="_blank"><i class="fa-brands fa-instagram-square"></i></a>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style>
footer {
  background-color: #000;
  color: #fff;
  text-align: center;
  padding: 30px 0;
}

footer a {
  text-decoration: none;
  color: #fff;
  display: inline-block;
  margin: 5px;
  font-size: 26px;
}
</style>