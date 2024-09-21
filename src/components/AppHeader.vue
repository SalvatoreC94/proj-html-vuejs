<template>
  <header>
    <!-- Header Superiore -->
    <div class="header-superiore ">
      <div>
        (001) 88451234 88455438
      </div>
      <nav>
        <ul class="">
          <li class="me-3">
            <a href="https://facebook.com" target="_blank">
              <i class="fab fa-facebook-f"></i>
            </a>
          </li>
          <li class="me-3">
            <a href="https://instagram.com" target="_blank">
              <i class="fab fa-instagram"></i>
            </a>
          </li>
          <li>
            <a href="https://pinterest.com" target="_blank">
              <i class="fab fa-pinterest-p"></i>
            </a>
          </li>
        </ul>
      </nav>
    </div>

    <!-- Header Inferiore -->
    <div class="header-inferiore">
      <div class="logo">
        <img src="/img/images/cropped-Group-39-2x.png" alt="Logo 1" />
      </div>
      <nav class="navbar">
        <ul class="nav">
          <li class="nav-item">
            <a class="nav-link" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Service</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Showcase</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Blog</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Contact</a>
          </li>
        </ul>
      </nav>
      <div class="purchase">
        <input type="button">Purchase
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'AppHeader',
};
</script>

<style scoped>
.purchase {
  width: 120px;
  height: 50px;
  border-radius: 25px;
  background-color: lightgreen;
  text-align: center;
  line-height: 50px;
  color: white;
  border: none;
  cursor: pointer;
}

.header-superiore {
  padding: 10px;
  background-color: grey;
  display: flex;
  justify-content: space-between;
}

.header-inferiore {
  padding: 20px;
  background-color: #e9ecef;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo img {
  height: 50px;
}

.navbar .nav {
  display: flex;
  list-style: none;
  padding: 0;
}

.nav-item .nav-link {
  margin: 0 15px;
  text-decoration: none;
  color: #000;
}

.header-superiore nav ul li i {
  font-size: 20px;
  color: white;
  
}
</style>
