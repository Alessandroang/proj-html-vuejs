<script>
export default {
  name: "AppHeader",
  data() {
    return {
      isDropdownOpen: false,
    };
  },
  methods: {
    // Funzione per attivare/disattivare il menu a tendina

    toggleDropdown() {
      this.isDropdownOpen = !this.isDropdownOpen;
    },
    // Funzione per attivare/disattivare il menu a scomparsa

    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
};
</script>

<template>
  <!-- Componente dell'intestazione -->
  <header class="header-content">
    <!-- Sezione del logo -->
    <div class="logo-container">
      <img
        src="../assets/img/logo-gobike.png"
        class="logo-img"
        alt="logo-header"
      />
    </div>

    <!-- Sezione del menu -->
    <div class="menu-container">
      <ul class="list">
        <!-- Elementi del menu -->
        <li><a href="#">Home</a></li>
        <li><a href="#">About Us</a></li>
        <!-- Elemento del menu a tendina -->
        <li class="nav-item dropdown" @click="toggleDropdown">
          <a
            class="nav-link dropdown-toggle"
            href="#"
            role="button"
            aria-expanded="false"
          >
            Trainings <i class="fas fa-chevron-down"></i>
          </a>
          <!-- Voci del menu a tendina -->
          <ul class="dropdown-menu" v-show="isDropdownOpen">
            <li><a class="dropdown-item" href="#">Riding Lessons</a></li>
            <li><a class="dropdown-item" href="#">Safe Driving</a></li>
            <li><a class="dropdown-item" href="#">Mountain Bike</a></li>
            <li><a class="dropdown-item" href="#">Trail Drive</a></li>
            <li><a class="dropdown-item" href="#">Pedaling</a></li>
          </ul>
        </li>

        <!-- Altri elementi del menu -->
        <li><a href="#">Packages</a></li>
        <li><a href="#">Blog</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </div>

    <!-- Menu a scomparsa -->
    <div class="hamburger-menu" @click="toggleMenu">
      <span></span>
      <span></span>
      <span></span>
    </div>

    <!-- Sezione del pulsante -->
    <div class="button-container">
      <button class="btn btn-black">
        Upcoming Events <i class="fas fa-arrow-right"></i>
      </button>
    </div>
  </header>
</template>

<style lang="scss" scoped>
.header-content {
  height: 100px;
  background-color: white;
  color: #fff;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.button-container {
  margin-left: 20px;
}

.btn-black {
  background-color: black;
  color: white;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  font-size: 18px;
}

.btn-black i {
  margin-left: 10px;
}

.logo-container {
  margin-right: 20px;
}

.menu-container {
  margin-left: 20px;
}

.list {
  display: flex;
  list-style-type: none;

  li {
    padding: 0px 10px;
  }

  a {
    text-decoration: none;
    color: black;
  }
}

.logo-img {
  width: 200px;
}

.hamburger-menu {
  width: 30px;
  height: 20px;
  position: relative;
  cursor: pointer;

  span {
    display: block;
    position: absolute;
    height: 2px;
    width: 100%;
    background: black;
    transition: transform 0.3s ease;
  }

  span:nth-child(1) {
    top: 0;
  }

  span:nth-child(2),
  span:nth-child(3) {
    top: 9px;
  }

  &.open span:nth-child(1) {
    transform: rotate(45deg);
    top: 9px;
  }

  &.open span:nth-child(2) {
    width: 0;
    opacity: 0;
  }

  &.open span:nth-child(3) {
    transform: rotate(-45deg);
    top: 9px;
  }
}
</style>
