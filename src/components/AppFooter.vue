<script>
export default {
  name: "AppFooter",
};
</script>

<template>
  <div class="menu-footer bg-black mt-4 text-white">
    <div class="container mt-4 d-flex justify-content-around">
      <div class="row">
        <div class="col-md-3 text-center">
          <div class="logo-footer">
            <img
              src="../assets/img/logo-footer-gobike.png"
              alt="logo-bg"
              class="logo-footer img-fluid"
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
          <div class="social-icons mb-2">
            <i class="fab fa-facebook"></i>
            <i class="fab fa-instagram"></i>
            <i class="fab fa-twitter"></i>
          </div>
        </div>

        <div class="col-md-3 text-center">
          <h3>Newsletter</h3>
          <p>Subscribe to our newsletter for updates</p>
          <form>
            <div class="mb-3">
              <input
                type="text"
                class="form-control"
                placeholder="Your email"
                aria-label="Your email"
              />
            </div>
            <div class="mb-3">
              <input
                type="text"
                class="form-control"
                placeholder="Subscribe"
                aria-label="Subscribe"
              />
            </div>
          </form>
        </div>

        <div class="col-md-3">
          <h3>Trainings</h3>
          <ul>
            <li><a href="">Riding lessons</a></li>
            <li><a href="">Safe driving</a></li>
            <li><a href="">Mountain Bike</a></li>
            <li><a href="">Trail Drive</a></li>
            <li><a href="">Pedaling</a></li>
          </ul>
        </div>

        <div class="col-md-3">
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
  </div>
</template>

<style scoped>
.logo-footer img {
  width: 100%;
}

.icons {
  .icon-item {
    display: flex;
    align-items: center;
    margin-bottom: 10px;

    i {
      font-size: 18px;
      margin-right: 10px;
    }

    span {
      font-size: 14px;
    }
  }
}

.social-icons {
  i {
    font-size: 24px;
    margin: 0 10px;
  }
}

.menu-footer {
  h3 {
    padding-top: 20px;
  }

  ul li {
    padding: 2px 0;

    a {
      color: white;

      &:hover {
        text-decoration: none;
      }
    }
  }
}
.menu-footer {
  ul {
    li {
      padding: 2px 0;
      position: relative;
      list-style: none;

      &:before {
        content: "—";
        margin-right: 5px;
      }

      a {
        color: white;
        text-decoration: none;
        &:hover {
          text-decoration: none;
        }
      }
    }
  }
}
</style>
