<script>
export default {
  data() {
    return {
      articles: [
        {
          date: "17.04.2023",
          imageSrc: "src/assets/img/news-bike5.jpg",
          title: "Road bike or mountain bike?",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut purus eget nunc ut dignissim cursus.",
        },
        {
          date: "05.05.2023",
          imageSrc: "src/assets/img/news-bike6.jpg",
          title: "How long does it take 5 km by bike",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut purus eget nunc ut dignissim cursus.",
        },
        {
          date: "29.12.2022",
          imageSrc: "src/assets/img/news-bike3.jpg",
          title: "How much should you cycle a day?",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut purus eget nunc ut dignissim cursus.",
        },
        {
          date: "12.03.2023",
          imageSrc: "src/assets/img/news-bike4.jpg",
          title: "What is mountain biking?",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut purus eget nunc ut dignissim cursus.",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="container mt-5 text-center">
    <h1 class="mb-3">Recent News & Articles</h1>
    <h5 class="mb-5">Useful information about bikes</h5>
    <div class="card-container">
      <div class="row justify-content-around">
        <div
          class="col-md-3 mb-4"
          v-for="(article, index) in articles"
          :key="index"
        >
          <div class="card">
            <img
              :src="article.imageSrc"
              class="card-img-top"
              alt="Article Image"
            />
            <div class="card-body text-center">
              <div class="card-date">{{ article.date }}</div>
              <h4 class="card-title">{{ article.title }}</h4>
              <p class="card-text">{{ article.text }}</p>
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
