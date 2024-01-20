<template>
  <div class="container mt-4">
    <div class="text-center mb-4">
      <h1>Our Expert Trainers</h1>
      <h5>Learn to ride a bike from the experts.</h5>
    </div>
    <div class="d-flex justify-content-center flex-wrap">
      <!-- Trainer 1 -->
      <div class="col-md-3 mb-4">
        <div class="card custom-card">
          <div class="card-overlay">
            <h5 class="card-title">John Der</h5>
            <h6 class="card-title">Biker</h6>
            <div class="social-icons">
              <i class="fab fa-facebook"></i>
              <i class="fab fa-twitter"></i>
              <i class="fab fa-instagram"></i>
            </div>
          </div>
          <img
            src="../../assets/img/biker1.jpg"
            class="card-img-top"
            alt="John Der - Biker"
          />
        </div>
      </div>

      <!-- Trainer 2 -->
      <div class="col-md-3 mb-4">
        <div class="card custom-card">
          <div class="card-overlay">
            <h5 class="card-title">Alice Rider</h5>
            <h6 class="card-title">Cycling Instructor</h6>
            <div class="social-icons">
              <i class="fab fa-facebook"></i>
              <i class="fab fa-twitter"></i>
              <i class="fab fa-instagram"></i>
            </div>
          </div>
          <img
            src="../../assets/img/biker2.jpg"
            class="card-img-top"
            alt="Alice Rider - Cycling Instructor"
          />
        </div>
      </div>

      <!-- Trainer 3 -->
      <div class="col-md-3 mb-4">
        <div class="card custom-card">
          <div class="card-overlay">
            <h5 class="card-title">Bob Cycleman</h5>
            <h6 class="card-title">Professional Biker</h6>
            <div class="social-icons">
              <i class="fab fa-facebook"></i>
              <i class="fab fa-twitter"></i>
              <i class="fab fa-instagram"></i>
            </div>
          </div>
          <img
            src="../../assets/img/biker3.jpg"
            class="card-img-top"
            alt="Bob Cycleman - Professional Biker"
          />
        </div>
      </div>

      <!-- Trainer 4 -->
      <div class="col-md-3 mb-4">
        <div class="card custom-card">
          <div class="card-overlay">
            <h5 class="card-title">Eva Cyclist</h5>
            <h6 class="card-title">Mountain Biking Expert</h6>
            <div class="social-icons">
              <i class="fab fa-facebook"></i>
              <i class="fab fa-twitter"></i>
              <i class="fab fa-instagram"></i>
            </div>
          </div>
          <img
            src="../../assets/img/biker4.jpg"
            class="card-img-top"
            alt="Eva Cyclist - Mountain Biking Expert"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.custom-card {
  position: relative;
  overflow: hidden;
  width: 14rem;
  margin-bottom: 20px;
}

.card-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.6);
  color: white;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  opacity: 0;
  transition: opacity 0.3s ease-in-out;
}

.custom-card:hover .card-overlay {
  opacity: 1;
}

.social-icons {
  display: flex;
  justify-content: center;
  margin-top: 10px;
}

.social-icons i {
  margin: 0 5px;
}
h1 {
  font-size: 3rem;
  font-weight: 700;
  color: black;
}
</style>

<style scoped>
.custom-card {
  position: relative;
  overflow: hidden;
  width: 14rem;
  margin-bottom: 20px;
}

.card-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.6);
  color: white;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  opacity: 0;
  transition: opacity 0.3s ease-in-out;
}

.custom-card:hover .card-overlay {
  opacity: 1;
}

.social-icons {
  display: flex;
  justify-content: center;
  margin-top: 10px;
}

.social-icons i {
  margin: 0 5px;
}
h1 {
  font-size: 3rem;
  font-weight: 700;
  color: black;
}
</style>
