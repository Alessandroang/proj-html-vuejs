<script>
export default {
  name: "AppFooter",
};
</script>

<template>
  <div class="menu-footer">
    <div class="menu-list">
      <div class="content-list">
        <div class="logo-footer">
          <img
            src="../assets/img/logo-footer-gobike.png"
            alt="logo-bg"
            class="logo-footer"
          />
        </div>
        <div class="icons">
          <div class="icon-item">
            <i class="fas fa-map-marker-alt"></i>
            <span>Civita Castellana ITA</span>
          </div>
          <div class="icon-item">
            <i class="fas fa-phone"></i>
            <span>+393664040</span>
          </div>
          <div class="icon-item">
            <i class="fas fa-envelope"></i>
            <span>ciao@ciao.com</span>
          </div>
        </div>
        <div class="social-icons">
          <i class="fab fa-facebook"></i>
          <i class="fab fa-instagram"></i>
          <i class="fab fa-twitter"></i>
        </div>
      </div>
      <div class="content-list">
        <h3>Newsletter</h3>
        <p>Subscribe to our newsletter for updates</p>
        <form class="container-fluid">
          <div class="mb-3">
            <input
              type="text"
              class="form-control form-control-lg"
              placeholder="Your email"
              aria-label="Your email"
              aria-describedby="basic-addon1"
            />
          </div>
          <div class="mb-3">
            <input
              type="text"
              class="form-control form-control-lg"
              placeholder="Subscribe"
              aria-label="Subscribe"
              aria-describedby="basic-addon2"
            />
          </div>
        </form>
      </div>

      <div class="content-list">
        <h3>Trainings</h3>
        <ul>
          <li><a href="">Riding lessons</a></li>
          <li><a href="">Safe driving</a></li>
          <li><a href="">Mountain Bike</a></li>
          <li><a href="">Trail Drive</a></li>
          <li><a href="">Pedaling</a></li>
        </ul>
      </div>
      <div class="content-list">
        <h3>Quick Links</h3>
        <ul>
          <li><a href="">Home</a></li>
          <li><a href="">About Us</a></li>
          <li><a href="">Blog</a></li>
          <li><a href="">Packages</a></li>
          <li><a href="">Contact</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.menu-footer {
  height: 300px;
  background-color: black;
  color: white;
}

.menu-footer a {
  color: white;
  text-decoration: none;
}
.menu-list ul {
  //   list-style-type: none;
  padding: 0;
}

.menu-list ul li {
  margin-bottom: 10px;
}

.menu-list ul li a {
  color: white;
  font-size: 14px;
}

.menu-list ul li a:hover {
  text-decoration: underline;
}

.menu-footer a:hover {
  text-decoration: underline;
}

.menu-footer button {
  color: white;
}

.logo-footer img {
  width: 200px;
  margin: 10px 0;
}
.icons {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin-top: 10px;
}
.social-icons {
  display: flex;
  justify-content: space-around;
}

.social-icons i {
  font-size: 24px;
  margin: 10px;
}

.icon-item {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}

.icon-item i {
  font-size: 18px;
  margin-right: 10px;
}

.icon-item span {
  font-size: 14px;
}

.menu-list {
  display: flex;
  justify-content: space-around;
  li {
    padding: 2px 0;
  }

  .content-list {
    padding: 20px;
    h3 {
      padding: 15px 0;
    }
  }
}
</style>
