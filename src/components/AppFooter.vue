<script>
export default {
  data() {
    return {
      footerData: {
        logo: {
          src: '/img/images/cropped-Group-39-2x.png',
          alt: 'Logo',
        },
        description: `While the lovely valley teems with vapour around me, and the meridian sun strikes 
                      the upper surface of the impenetrable foliage of my trees.`,
        quickLinks: {
          title: 'Quick Links',
          items: ['Careers', 'News', 'Terms of use', 'Privacy Projects', 'About', 'Contact'],
        },
        contact: {
          title: 'Contact',
          name: 'Patricia C. Amedee',
          address: '4401 Waldeck Street',
          city: 'Grapevine Nashville, TX 76051',
          email: 'info@yourdomain.com',
          phone: '+99 (0) 101 0000 888',
        },
        map: {
          title: 'Location on Map',
          src: 'https://maps.app.goo.gl/fgGLFtCFoUrMT7Nf9',
        },
      },
    };
  },
};
</script>

<template>
  <footer class="footer ">
    <!-- Colonna 1: Logo e descrizione -->
    <div class="footer-column">
      <img :src="footerData.logo.src" :alt="footerData.logo.alt" class="footer-logo" />
      <p>{{ footerData.description }}</p>
    </div>

    <!-- Colonna 2: Quick Links -->
    <div class="footer-column">
      <h2>{{ footerData.quickLinks.title }}</h2>
      <ul>
        <li v-for="(link, index) in footerData.quickLinks.items" :key="index">{{ link }}</li>
      </ul>
    </div>

    <!-- Colonna 3: Contatti -->
    <div class="footer-column">
      <h2>{{ footerData.contact.title }}</h2>
      <ul>
        <li>{{ footerData.contact.name }}</li>
        <li>{{ footerData.contact.address }}</li>
        <li>{{ footerData.contact.city }}</li>
        <li>{{ footerData.contact.email }}</li>
        <li>{{ footerData.contact.phone }}</li>
      </ul>
    </div>

    <!-- Colonna 4: Mappa -->
    <div class="footer-column">
      <h2>{{ footerData.map.title }}</h2>
      <div class="map">
        <iframe src="https://www.google.com/maps/embed?pb=!1m10!1m8!1m3!1d48398.917260584254!2d-73.979681!3d40.69748800000001!3m2!1i1024!2i768!4f13.1!5e0!3m2!1sit!2sit!4v1727081685232!5m2!1sit!2sit"
         width="350"
         height="200" 
         style="border:0;" 
         allowfullscreen="" 
         loading="lazy" 
         referrerpolicy="no-referrer-when-downgrade">
        </iframe>
      </div>
    </div>
  </footer>
</template>


<style scoped>
.footer {
  padding: 20px;
  background-color: #f8f9fa;
  color: #333;
  display: flex;
}

.footer-column {
  flex: 1;
  padding: 0 20px;
}

.footer-column h4 {
  color: #333;
  font-weight: bold;
  margin-bottom: 15px;
}

.footer-column ul {
  list-style: none;
  padding: 0;
}

.footer-column ul li {
  margin-bottom: 10px;
  color: #555;
}

.footer-logo {
  width: 200px;
  margin-bottom: 15px;
}

.map iframe {
  width: 100%;
  border-radius: 8px;
 
}


</style>
