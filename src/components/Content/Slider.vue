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
          <div class="carousel-caption text-start">
            <h4>Professional Cycling Club</h4>
            <p>Learn cycling from the pros</p>
            <button class="btn btn-black">Learn More</button>
          </div>
        </div>
        <!-- Seconda slide -->
        <div class="carousel-item">
          <img
            src="../../assets/img/slider-bike-4.jpg"
            class="d-block w-100"
            alt="..."
          />
          <div class="carousel-caption text-start">
            <h4>Professional Cycling Club</h4>
            <p>Learn cycling from the pros</p>
            <button class="btn btn-black">Learn More</button>
          </div>
        </div>
        <!-- Terza slide -->
        <div class="carousel-item">
          <img
            src="../../assets/img/slider-bike-12.jpg"
            class="d-block w-100"
            alt="..."
          />
          <div class="carousel-caption text-start">
            <h4>Professional Cycling Club</h4>
            <p>Learn cycling from the pros</p>
            <button class="btn btn-black">Learn More</button>
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
  <div class="container mt-5">
    <div class="row">
      <div class="col-md-6 sfondo-div">
        <img
          src="../../assets/img/bike-player.png"
          alt="Immagine"
          class="img-fluid"
        />
      </div>
      <div class="col-md-6">
        <div class="d-flex flex-column align-items-start">
          <!-- Titolo -->
          <h1>Do you want to be a professional cyclist?</h1>

          <!-- Sottotitolo -->
          <h6>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim sed
            possimus quaerat fuga. Aperiam, officia rerum? Illo repellendus
            inventore ipsam odio quisquam nisi, distinctio voluptatum optio hic
            minima, perspiciatis reiciendis!
          </h6>

          <img
            src="../../assets/img/divider.jpg"
            alt="Divider"
            class="divider-img mt-5"
          />

          <div class="d-flex flex-column mt-5">
            <i class="fas fa-hard-hat fa-2xl mb-5"></i>

            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Atque
              suscipit optio deleniti beatae, tempore inventore fuga sint,
            </p>
          </div>

          <div class="d-flex flex-column mt-5">
            <i class="fas fa-bicycle fa-2xl mb-5"></i>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Atque
              suscipit optio deleniti beatae, tempore inventore fuga sint,
            </p>
          </div>
          <div class="button-container">
            <button class="btn btn-black btn-lg">
              Get to know us
              <i class="fas fa-arrow-right"></i>
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.carousel-item {
  height: 500px;
}
.carousel-item img {
  height: 100%;
  width: 100%;
  object-fit: cover;
}
.carousel-caption {
  top: 200px;
}
.divider-img {
  width: 100px;
  padding-top: 10px;
}
.sfondo-div {
  background-image: url("../../assets/img/bike-circle.png");
  background-size: 100%;
  background-repeat: no-repeat;
}

.button-container {
  margin-right: 20px;
}

.btn-black {
  background-color: black;
  color: white;
}
</style>
