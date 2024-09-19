<script>
export default {
  name: 'AppHeader',
};
</script>

<template>
  <header>
    <!-- Header Superiore -->
    <div class="header-superiore d-flex justify-content-between">
      <div>Elemento Sinistra</div>
      <div>Elemento Destra</div>
    </div>

    <!-- Header Inferiore -->
    <div class="header-inferiore d-flex justify-content-between align-items-center">
      <div class="logo">
        <img src="" alt="Logo 1" />
      </div>
      <nav class="navbar">
        <ul class="nav">
          <li class="nav-item">
            <a class="nav-link" href="#">Home</a>
          </li><li class="nav-item">
            <a class="nav-link" href="#">Home</a>
          </li><li class="nav-item">
            <a class="nav-link" href="#">Home</a>
          </li><li class="nav-item">
            <a class="nav-link" href="#">Home</a>
          </li><li class="nav-item">
            <a class="nav-link" href="#">Home</a>
          </li>
          
        </ul>
      </nav>
      <div class="logo">
        <img src="" alt="Logo 2" />
      </div>
    </div>
  </header>
</template>


<style scoped>
.header-superiore {
  padding: 10px;
  background-color: #f8f9fa;
  display: flex;
  justify-content: space-between;
}

.header-inferiore {
  padding: 20px;
  background-color: #e9ecef;
  display: flex;
  justify-content: space-between;
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
  
</style>
