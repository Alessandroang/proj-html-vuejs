<template>
  <div class="container mt-4">
    <div class="text-center mb-4">
      <h1>Our Professional Cycling Trainings</h1>
      <h4>Learn from the mountain bike expert</h4>
    </div>
    <div class="d-flex justify-content-center flex-wrap">
      <div class="col-md-3">
        <div class="card custom-card">
          <div class="card-overlay">
            <div class="card-label">Riding Lesson</div>
            <img
              src="../../assets/img/training-box-1.jpg"
              class="card-img-top"
              alt="Card image"
            />
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card custom-card">
          <div class="card-overlay">
            <div class="card-label">Safe Driving</div>
            <img
              src="../../assets/img/training-box-2.jpg"
              class="card-img-top"
              alt="Card image"
            />
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card custom-card">
          <div class="card-overlay">
            <div class="card-label">Mountain bike</div>
            <img
              src="../../assets/img/training-box-3.jpg"
              class="card-img-top"
              alt="Card image"
            />
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card custom-card">
          <div class="card-overlay">
            <div class="card-label">Trail Drive</div>
            <img
              src="../../assets/img/training-box-4.jpg"
              class="card-img-top"
              alt="Card image"
            />
          </div>
        </div>
      </div>
      <button type="button" class="btn btn-light mx-2">
        <i class="fas fa-arrow-left text-dark"></i>
      </button>
      <button type="button" class="btn btn-light mx-2">
        <i class="fas fa-arrow-right text-dark"></i>
      </button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: 16rem;
  margin-bottom: 20px;
  border-radius: 10px;
}

.custom-card {
  border: 5px solid #000;
  position: relative;
}

.card-overlay {
  position: relative;
  overflow: hidden;
  border-radius: 10px;
}

.card-overlay:hover {
  background-color: rgba(0, 0, 0, 0.6);
}

.card-label {
  position: absolute;
  top: 10px;
  left: 10px;
  color: white;
  background: rgba(0, 0, 0, 0.5);
  padding: 5px 10px;
  font-size: 14px;
}

.card img {
  max-width: 100%;
}

h1 {
  font-size: 3rem;
  font-weight: 700;
  color: black;
}
</style>
