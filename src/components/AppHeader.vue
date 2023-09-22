<script>
export default {
  name: "AppHeader",
};
</script>

<template>
  <!-- Componente dell'intestazione -->
  <header class="header-content navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <!-- Logo -->
      <a class="navbar-brand" href="#">
        <img
          src="../assets/img/logo-gobike.png"
          class="logo-img img-fluid"
          alt="logo-header"
        />
      </a>

      <!-- Toggle button per dispositivi mobili -->
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Menu -->
      <div
        class="collapse navbar-collapse justify-content-center"
        id="navbarNav"
      >
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link" href="#">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="#">About Us</a></li>

          <!-- Elemento del menu a tendina -->
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              id="navbarDropdown"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              Trainings
            </a>

            <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
              <li><a class="dropdown-item" href="#">Riding Lessons</a></li>
              <li><a class="dropdown-item" href="#">Safe Driving</a></li>
              <li><a class="dropdown-item" href="#">Mountain Bike</a></li>
              <li><a class="dropdown-item" href="#">Trail Drive</a></li>
              <li><a class="dropdown-item" href="#">Pedaling</a></li>
            </ul>
          </li>

          <li class="nav-item"><a class="nav-link" href="#">Packages</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Blog</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Contact</a></li>
        </ul>
      </div>

      <!-- Sezione del pulsante -->
      <div class="button-container">
        <button class="btn btn-black btn-lg">
          <i class="fas fa-hard-hat"></i> Upcoming Events
          <i class="fas fa-arrow-right"></i>
        </button>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo-img {
  width: 200px;
}

.button-container {
  margin-right: 20px;
}

.btn-black {
  background-color: black;
  color: white;
}

.nav-item {
  font-weight: 700;
}
</style>
