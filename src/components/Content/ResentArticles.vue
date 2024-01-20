<template>
  <div class="container mt-5 text-center">
    <h1 class="mb-3">Recent News & Articles</h1>
    <h5 class="mb-5">Useful information about bikes</h5>
    <div class="card-container">
      <div class="row justify-content-around">
        <!-- Article 1 -->
        <div class="col-md-3 mb-4">
          <div class="card">
            <img
              src="../../assets/img/news-bike5.jpg"
              class="card-img-top"
              alt="Road bike or mountain bike?"
            />
            <div class="card-body text-center">
              <div class="card-date">17.04.2023</div>
              <h4 class="card-title">Road bike or mountain bike?</h4>
              <p class="card-text">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut
                purus eget nunc ut dignissim cursus.
              </p>
              <div class="button-more">
                <button class="btn btn-dark">More</button>
              </div>
            </div>
          </div>
        </div>

        <!-- Article 2 -->
        <div class="col-md-3 mb-4">
          <div class="card">
            <img
              src="../../assets/img/news-bike6.jpg"
              class="card-img-top"
              alt="How long does it take 5 km by bike"
            />
            <div class="card-body text-center">
              <div class="card-date">05.05.2023</div>
              <h4 class="card-title">How long does it take 5 km by bike</h4>
              <p class="card-text">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut
                purus eget nunc ut dignissim cursus.
              </p>
              <div class="button-more">
                <button class="btn btn-dark">More</button>
              </div>
            </div>
          </div>
        </div>

        <!-- Article 3 -->
        <div class="col-md-3 mb-4">
          <div class="card">
            <img
              src="../../assets/img/news-bike3.jpg"
              class="card-img-top"
              alt="How much should you cycle a day?"
            />
            <div class="card-body text-center">
              <div class="card-date">29.12.2022</div>
              <h4 class="card-title">How much should you cycle a day?</h4>
              <p class="card-text">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut
                purus eget nunc ut dignissim cursus.
              </p>
              <div class="button-more">
                <button class="btn btn-dark">More</button>
              </div>
            </div>
          </div>
        </div>

        <!-- Article 4 -->
        <div class="col-md-3 mb-4">
          <div class="card">
            <img
              src="../../assets/img/news-bike4.jpg"
              class="card-img-top"
              alt="What is mountain biking?"
            />
            <div class="card-body text-center">
              <div class="card-date">12.03.2023</div>
              <h4 class="card-title">What is mountain biking?</h4>
              <p class="card-text">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut
                purus eget nunc ut dignissim cursus.
              </p>
              <div class="button-more">
                <button class="btn btn-dark">More</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card-container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.card {
  border: 1px solid #ccc;
  border-radius: 5px;
  margin-bottom: 20px;
  position: relative;
  overflow: hidden;
  box-shadow: 0 0 30px rgba(0, 0, 0, 0.7);
}
</style>
