<template>
  <div class="container">
    <div class="text-center mb-4">
      <h1>Our Professional Cycling Trainings</h1>
      <h6>Learn from the mountain bike expert</h6>
    </div>
    <div class="d-flex justify-content-center flex-wrap">
      <div class="col-md-3">
        <div class="card custom-card">
          <img
            src="../../assets/img/training-box-1.jpg"
            class="card-img-top"
            alt="Card image"
          />
          <div class="card-body">
            <h5 class="card-title">Card 1</h5>
            <p class="card-text">Description for card 1</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card custom-card">
          <img
            src="../../assets/img/training-box-2.jpg"
            class="card-img-top"
            alt="Card image"
          />
          <div class="card-body">
            <h5 class="card-title">Card 2</h5>
            <p class="card-text">Description for card 2</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card custom-card">
          <img
            src="../../assets/img/training-box-3.jpg"
            class="card-img-top"
            alt="Card image"
          />
          <div class="card-body">
            <h5 class="card-title">Card 3</h5>
            <p class="card-text">Description for card 3</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card custom-card">
          <img
            src="../../assets/img/training-box-4.jpg"
            class="card-img-top"
            alt="Card image"
          />
          <div class="card-body">
            <h5 class="card-title">Card 4</h5>
            <p class="card-text">Description for card 4</p>
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

<style scoped>
.container h2 {
  color: #333;
  font-size: 24px;
  margin-bottom: 20px;
}

.card {
  width: 18rem;
  margin-bottom: 20px;
}

.custom-card {
  border: 5px solid #000;
}
</style>
