<template>
  <div class="container-fluid">
    <div
      id="carouselExampleCaptions"
      class="carousel slide"
      data-bs-ride="false"
    >
      <div class="carousel-indicators">
        <button
          type="button"
          data-bs-target="#carouselExampleCaptions"
          data-bs-slide-to="0"
          class="active"
          aria-current="true"
          aria-label="Slide 1"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleCaptions"
          data-bs-slide-to="1"
          aria-label="Slide 2"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleCaptions"
          data-bs-slide-to="2"
          aria-label="Slide 3"
        ></button>
      </div>
      <div class="carousel-inner">
        <!-- Prima slide -->
        <div class="carousel-item active">
          <img
            src="../../assets/img/slider-bike-9.jpg"
            class="d-block w-100"
            alt="..."
          />
          <div class="carousel-caption">
            <h4>Professional Cycling Club</h4>
            <p>Learn cycling from the pros</p>
          </div>
        </div>
        <!-- Seconda slide -->
        <div class="carousel-item">
          <img
            src="../../assets/img/slider-bike-4.jpg"
            class="d-block w-100"
            alt="..."
          />
          <div class="carousel-caption">
            <h4>Professional Cycling Club</h4>
            <p>Learn cycling from the pros</p>
          </div>
        </div>
        <!-- Terza slide -->
        <div class="carousel-item">
          <img
            src="../../assets/img/slider-bike-12.jpg"
            class="d-block w-100"
            alt="..."
          />
          <div class="carousel-caption">
            <h4>Professional Cycling Club</h4>
            <p>Learn cycling from the pros</p>
          </div>
        </div>
      </div>
      <!-- Controlli per la navigazione -->
      <button
        class="carousel-control-prev"
        type="button"
        @click="showPreviousSlide"
        data-bs-target="#carouselExampleCaptions"
        data-bs-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button
        class="carousel-control-next"
        type="button"
        @click="showNextSlide"
        data-bs-target="#carouselExampleCaptions"
        data-bs-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    showNextSlide() {
      const carousel = new bootstrap.Carousel(
        document.getElementById("carouselExampleCaptions")
      );
      carousel.next();
    },
    showPreviousSlide() {
      const carousel = new bootstrap.Carousel(
        document.getElementById("carouselExampleCaptions")
      );
      carousel.prev();
    },
  },
};
</script>

<style lang="scss">
.carousel-item {
  height: 400px;
}
.carousel-item img {
  height: 100%;
  width: 100%;
  object-fit: cover;
}
</style>
