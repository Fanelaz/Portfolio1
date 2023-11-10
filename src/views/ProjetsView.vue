<template>
  <body>
    <h1>Projets</h1>
    <div class="cv">
      <figure class="card">
        <img src="../assets/CV.png" alt="image" class="card-image" />
        <figcaption class="card-body">
          <h2 class="card-title">CV HTML</h2>
          <p class="card-description">
            Mon premier Projets en HTML/CSS : Mon CV
          </p>
          <div class="exemple">
            <a href="https://github.com/Fanelaz/CV" target="_blank">
            <input
              class="card-description"
              type="button"
              value="Github"
            />
            </a>
          </div>


        </figcaption>
      </figure>
    </div>
  </body>
</template>

<script>
export default {
  name: "Projets",
};
</script>

<style scoped>
body {
  width: auto;
  height: 1080px;
}

.cv {
  padding-left: 250px;
}

.card {
  position: relative;
  width: 350px;
  height: 250px;
  background: #000;
  overflow: hidden;
}

.card-image {
  height: 100%;
  width: 100%;
  object-fit: cover;
  scale: 1.5;
  transition: opacity 0.25s, scale 0.35s;
}

.card:hover .card-image {
  opacity: 0.5;
  scale: 1;
}
.card-body {
  position: absolute;
  inset: 0;
  padding: 50px;
  color: #fff;
  text-align: center;
  flex-direction: column;
  align-items: center;
  row-gap: 15px;
  justify-content: center;
}
.card-body::before {
  content: "";
  position: absolute;
  inset: 20px;
  border: 2px solid #fff;
  opacity: 0;
  scale: 1.25;
  transition: opacity 0.25s, scale 0.35s;
}

.card:hover .card-body::before {
  opacity: 1;
  scale: 1;
}

.card-title {
  letter-spacing: 1px;
  text-transform: uppercase;
  text-shadow: 1px 1px 10px rgba(0, 0, 0, 0.5);
}

.card-description {
  font-size: 14px;
  opacity: 0;
  transition: opacity 0.25s, translate 0.25s;
}

.card:hover .card-description {
  opacity: 1;
  translate: 0;
}

/* Sub for more content  */
</style>
