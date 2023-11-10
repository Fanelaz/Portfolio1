<template>
  <div class="footer">
    <div class="social">
      <a href="https://github.com/Fanelaz"
        ><img src="../assets/icons8-github-50.png" alt="Github Logo"
      /></a>
      <a href="https://www.linkedin.com/in/mickaël-le-breton-b0b640293/"
        ><img src="../assets/icons8-linkedin-50.png" alt="Linkedin Logo"
      /></a>
    </div>
    <a href="https://www.google.fr/maps/place/Rue+Robert+Masson,+27300+Bernay/@49.0912242,0.5783382,17z/data=!3m1!4b1!4m6!3m5!1s0x47e1a3b9d6b32569:0x1814ed80898552d6!8m2!3d49.0912207!4d0.5809131!16s%2Fg%2F11hbq9gt5_?entry=ttu" target="_blank">
      <div class="adress">
        <h3>122 rue robert Masson</h3>
        <h3>Bernay</h3>
        <h3>27300</h3>
      </div>
    </a>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>


.footer {
  background-color: #555;
  height: 250px;
  width: 100%;
}

h1 {
  color: black;
}

.social {
  display: flex;
  align-items: center;
  justify-content: center;
  padding-top: 50px;
}

.social a {
  margin: 0 50px;
}

.social a:hover {
  box-shadow: 10px 5px 5px black;
}

.adress {
  display: block;
  text-align: center;
  border-style: solid;
  width: 250px;
  float: right;
  background-color: #555;
}
</style>
