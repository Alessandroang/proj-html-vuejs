<script>
export default {
  data() {
    return {
      hoveredCard: null,

      cards: [
        {
          title: "Basic",
          description: "Learn to ride a bike from the professionals",
          features: [
            { text: "Phone Mountainer bike training", isFeatureTrue: true },
            { text: "Remote Excellent bike service", isFeatureTrue: true },
            { text: "Onsite Safe cycling training", isFeatureTrue: true },
            { text: "Saafety helmet on bike", isFeatureTrue: false },
            { text: "Free bikes for children", isFeatureTrue: false },
          ],
          price: "€ 19,99/mese",
        },
        {
          title: "Standard",
          description: "Learn to ride a bike from the professionals",
          features: [
            { text: "Phone Mountainer bike training", isFeatureTrue: true },
            { text: "Remote Excellent bike service", isFeatureTrue: true },
            { text: "Onsite Safe cycling training", isFeatureTrue: true },
            { text: "Saafety helmet on bike", isFeatureTrue: false },
            { text: "Free bikes for children", isFeatureTrue: false },
          ],
          price: "€ 39,99/mese",
        },
        {
          title: "Premium",
          description: "Learn to ride a bike from the professionals",
          features: [
            { text: "Phone Mountainer bike training", isFeatureTrue: true },
            { text: "Remote Excellent bike service", isFeatureTrue: true },
            { text: "Onsite Safe cycling training", isFeatureTrue: true },
            { text: "Saafety helmet on bike", isFeatureTrue: false },
            { text: "Free bikes for children", isFeatureTrue: false },
          ],
          price: "€ 69,99/mese",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="container">
    <div class="titles">
      <div class="square bg-black">
        <div class="square-white">
          <i class="fa-solid fa-shop-lock fa-beat fa-xl text-white"></i>
        </div>
      </div>
      <div class="title">Special Packs</div>
      <div class="subtitle">Select a pricing plan to get more</div>
    </div>

    <div class="row mt-4">
      <!-- Itera su ogni card nell'array e visualizzala -->
      <div class="col-md-4" v-for="(card, index) in cards" :key="index">
        <div
          class="card"
          @mouseover="hoveredCard = index"
          @mouseleave="hoveredCard = null"
        >
          <div class="card-content">
            <div class="card-header">
              <div class="text-center">
                <i class="fa-solid fa-handshake-simple fa-2xl mb-4"></i>
                <h3 class="mb-4">{{ card.title }}</h3>
                <p class="mb-4">{{ card.description }}</p>
              </div>
            </div>
            <div class="card-body">
              <ul>
                <li v-for="(feature, index) in card.features" :key="index">
                  <i
                    :class="{
                      'fa-solid': true,
                      'fa-check': feature.isFeatureTrue,
                      'fa-times': !feature.isFeatureTrue,
                      'me-2': true,
                    }"
                  ></i>
                  {{ feature.text }}
                </li>
              </ul>
            </div>
          </div>
          <div class="overlay" :class="{ active: hoveredCard === index }">
            <div class="overlay-content">
              <h2>{{ card.title }}</h2>
              <p>{{ card.price }}</p>
              <button class="btn btn-dark">Acquista ora</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  border: 1px solid #ccc;
  border-radius: 5px;
  margin-bottom: 20px;
  position: relative;
  overflow: hidden;
  box-shadow: 0 0 30px rgba(0, 0, 0, 0.7);
}

.card-content {
  transition: transform 0.3s;
}

.card:hover .card-content {
  transform: translateY(-50%);
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  padding: 20px;
  background-color: rgba(0, 0, 0, 0.8);
  color: white;
  text-align: center;
  transform: scale(0);
  transform-origin: center;
  transition: transform 0.3s;
}

.overlay.active {
  transform: scale(1);
}

.overlay-content {
  position: relative;
  top: 50%;
  transform: translateY(-50%);
}

.card-header {
  background-color: black;
  color: white;
  padding: 20px;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
}

.text-center {
  text-align: center;
}

ul {
  list-style-type: none;
  padding: 0;
}

ul li {
  margin-bottom: 10px;
  text-align: center;
}

ul li:not(:last-child) {
  border-bottom: 1px solid #ccc;
}

.titles {
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
}

.square {
  width: 10rem;
  height: 10rem;
  border: 3px solid white;
  display: flex;
  justify-content: center;
  align-items: center;
}

.square-white {
  border: 3px solid white;
  width: 6rem;
  height: 6rem;
  display: flex;
  justify-content: center;
  align-items: center;
}

.title {
  font-size: 3rem;
  font-weight: 700;
  color: black;
}

.subtitle {
  font-size: 2rem;
  font-weight: 400;
  color: black;
}
</style>
