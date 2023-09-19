<template>
  <header class="header-content">
    <div class="logo-container">
      <img
        src="../assets/img/logo-gobike.png"
        class="logo-img"
        alt="logo-header"
      />
    </div>
    <div class="menu-container">
      <ul class="list">
        <li><a href="">Home</a></li>
        <li><a href="">About Us</a></li>
        <li><a href="">Trainings</a></li>
        <li><a href="">Packages</a></li>
        <li><a href="">Blog</a></li>
        <li><a href="">Contact</a></li>
      </ul>
    </div>
    <div class="hamburger-menu" @click="toggleMenu">
      <span></span>
      <span></span>
      <span></span>
    </div>
    <div class="button-container">
      <button class="btn btn-black">
        Upcoming Events<i class="fas fa-arrow-right"></i>
      </button>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
};
</script>

<style lang="scss" scoped>
.header-content {
  background-color: white;
  color: #fff;
  padding: 10px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.button-container {
  margin-left: 20px;
}

.btn-black {
  background-color: black;
  color: white;
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
