<template>
  <div class="container mt-5">
    <div class="titles">
      <div class="title">Resent News & Articles</div>
      <div class="subtitle">Useful information about bikes</div>
    </div>

    <div class="container mt-5">
      <div class="row justify-content-around">
        <div class="col-md-3 mb-4">
          <div class="card">
            <img
              src="../../assets/img/news-bike5.jpg"
              class="card-img-top"
              alt="Article Image"
            />
            <div class="card-body text-center">
              <div class="card-date">17.04.2023</div>
              <h3 class="card-title">Road bike or mountain bike?</h3>
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

        <div class="col-md-3 mb-4">
          <div class="card">
            <img
              src="../../assets/img/news-bike6.jpg"
              class="card-img-top"
              alt="Article Image"
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

        <div class="col-md-3 mb-4">
          <div class="card">
            <img
              src="../../assets/img/news-bike3.jpg"
              class="card-img-top"
              alt="Article Image"
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

        <div class="col-md-3 mb-4">
          <div class="card">
            <img
              src="../../assets/img/news-bike4.jpg"
              class="card-img-top"
              alt="Article Image"
            />
            <div class="card-body text-center">
              <div class="card-date">12.03.2023</div>
              <h3 class="card-title">What is mountain biking?</h3>
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
.card {
  border: 1px solid #ccc;
  border-radius: 5px;
  margin-bottom: 20px;
  position: relative;
  overflow: hidden;
  box-shadow: 0 0 30px rgba(0, 0, 0, 0.7);
}
.titles {
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;

  .title {
    font-size: 3rem;
    font-weight: 700;
    color: black;
  }

  .subtitle {
    font-size: 1.875rem;
    font-weight: 400;
    color: black;
  }
}
</style>
