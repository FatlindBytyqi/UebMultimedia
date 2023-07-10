<template>
    <div id="carouselExampleIndicators" class="carousel slide">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="https://www.leparisien.fr/resizer/GngA8tJnu0yArs6-dYqAhB1WbT8=/arc-anglerfish-eu-central-1-prod-leparisien/public/MK63RBQRENH6HDA3W2GTTT2SYE.jpg" class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="../../assets/judo.png" class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="../../assets/akil2.jpg" class="d-block w-100" alt="...">
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
</template>
<style>
.carousel-inner {
  max-width: 1200%;
  max-height: 800px; /* Adjust the desired height */
  object-fit: cover;
}
</style>