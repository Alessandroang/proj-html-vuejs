<script>
export default {
  data() {
    return {
      showLoader: true, // Mostra il loader all'inizio
      isFlashing: false, // Flag per l'effetto di lampeggiamento
    };
  },
  mounted() {
    // Lampeggia l'immagine ogni 1 secondo
    setInterval(() => {
      this.isFlashing = !this.isFlashing;
    }, 300);

    setTimeout(() => {
      this.showLoader = false;
    }, 1500);
  },
};
</script>

<template>
  <div v-if="showLoader" class="loader">
    <img
      src="../../assets/img/loader-gobike.png"
      alt="Loading"
      :class="{ flashing: isFlashing }"
    />
  </div>
</template>

<style scoped>
.loader {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.loader img {
  width: 100px;
}

.flashing {
  animation: flash 0.5s infinite alternate;
}

@keyframes flash {
  0% {
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
