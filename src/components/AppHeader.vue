<script>
export default {
  name: 'AppHeader',
  data() {
    return {
      // Link di navigazione dinamici
      navLinks: [
        { name: 'Home', url: '/' },
        { name: 'About', url: '/about' },
        { name: 'Services', url: '/services' },
        { name: 'Portfolio', url: '/portfolio' },
        { name: 'Blog', url: '/blog' },
        { name: 'Contact', url: '/contact' }
      ],
      // Link social dinamici
      socialLinks: [
        { icon: 'fab fa-facebook-f', url: 'https://facebook.com' },
        { icon: 'fab fa-instagram', url: 'https://instagram.com' },
        { icon: 'fab fa-pinterest-p', url: 'https://pinterest.com' }
      ]
    };
  }
};
</script>

<template>
  <header>
    <!-- Header Superiore -->
    <div class="header-superiore">
      <div class="contact-info">
        (001) 88451234 88455438
      </div>
      <nav class="social-links">
        <ul>
          <li class="me-3" v-for="(link, index) in socialLinks" :key="index">
            <a :href="link.url" target="_blank">
              <i :class="link.icon"></i>
            </a>
          </li>
        </ul>
      </nav>
    </div>

    <!-- Header Inferiore -->
    <div class="header-inferiore">
      <!-- Logo -->
      <div class="logo">
        <img src="/img/images/cropped-Group-39-2x.png" alt="Logo" />
      </div>

      <!-- Menu di Navigazione -->
      <nav class="navbar">
        <ul class="nav">
          <li class="nav-item" v-for="(item, index) in navLinks" :key="index">
            <a class="nav-link" :href="item.url">{{ item.name }}</a>
          </li>
        </ul>
      </nav>

      <!-- Pulsante "Purchase" -->
      <div class="purchase">
        <button>Purchase</button>
      </div>
    </div>
  </header>
</template>

<style scoped>
/* Stili Generali */
header {
  font-family: Arial, sans-serif;
  position: fixed;
  width: 100%;
  z-index: 1000; 
  background-color: white; 
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

/* Header Superiore */
.header-superiore {
  background-color: #333;
  padding: 10px 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.contact-info {
  color: #fff;
}

.social-links ul {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

.social-links li a {
  color: #fff;
  font-size: 18px;
  text-decoration: none;
}

.social-links li a:hover {
  color: lightgreen;
}

/* Header Inferiore */
.header-inferiore {
  background-color: #f8f9fa;
  padding: 20px 40px;
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
  margin: 0;
}

.nav-item .nav-link {
  margin: 0 15px;
  text-decoration: none;
  color: #333;
  font-size: 16px;
  font-weight: bold;
}

.nav-item .nav-link:hover {
  color: #007bff;
}


.purchase button {
  background-color: lightgreen;
  border: none;
  border-radius: 25px;
  color: #fff;
  padding: 10px 20px;
  cursor: pointer;
  font-size: 16px;
}

.purchase button:hover {
  background-color: #28a745;
}
</style>
