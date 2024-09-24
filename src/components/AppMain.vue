<script>
export default {
  name: 'HomePage',
  data() {
    return {
      services: [
        { title: 'Speed Optimization', description: 'Optimize your website speed to improve user experience.' },
        { title: 'Cloud Solutions', description: 'Secure and scalable cloud solutions to grow your business.' },
        { title: 'Website Design', description: 'Beautiful and responsive designs for your online presence.' },
        { title: 'Online Marketing', description: 'Strategic marketing campaigns to boost your brand visibility.' }
      ],
      projects: [
        { src: '/public/img/images/ina-soulis-227104-unsplash-1024x1024.jpg', alt: 'Project 1' },
        { src: '/public/img/images/sunisa-misa-531163-unsplash-1024x1024.jpg', alt: 'Project 2' },
        { src: '/public/img/images/355H-1024x1024.jpg', alt: 'Project 3' },
        { src: '/public/img/images/photo-1448932252197-d19750584e56-1024x1024.jpg', alt: 'Project 4' },
        { src: '/public/img/images/business-competition-PB366D8-1024x1024.jpg', alt: 'Project 5' },
        { src: '/public/img/images/cozy-sofa-in-living-room-PQR5AB9-1024x1024.jpg', alt: 'Project 6' },
        { src: '/public/img/images/aa9a4539-PQGJ7HU-1024x1024.jpg', alt: 'Project 7' },
        { src: '/public/img/images/cody-davis-253928-unsplash-1024x1024.jpg', alt: 'Project 8' }
      ],
      blogPosts: [
        { 
          title: 'Marketing Ideas', 
          image: '/public/img/images/serious-businesswoman-with-documents-talking-on-P9Q6LX6-1024.jpg', 
          date: 'May 24, 2018 - Alex', 
          excerpt: 'Explore new marketing strategies to increase your sales.' 
        },
        { 
          title: 'Rest During Working Hours', 
          image: '/public/img/images/Businessman-at-the-desk-in-his-office-resting--1024x768.jpg', 
          date: 'May 24, 2018 - Alex', 
          excerpt: 'Understanding the balance between work and rest.' 
        },
        { 
          title: 'Develop Your Startup Idea', 
          image: '/public/img/images/simple-home-office-with-tree-PBXRXYB-large-1024x768.jpg', 
          date: 'May 24, 2018 - Alex', 
          excerpt: 'From idea to execution: steps to start your business.' 
        }
      ],
      pricing:[
        { title: 'Designing', cost: '$10 / Design', features: ['Creative design enabled', 'Vibrant color usage', 'Eye-catching design', 'Extreme typography', 'Exceptional design'] },
        { title: 'Development', cost: '$15 / Design', features: ['Creative design enabled', 'Vibrant color usage', 'Eye-catching design', 'Extreme typography', 'Exceptional design'] },
        { title: 'SEO', cost: '$10 / Product', features: ['Creative design enabled', 'Vibrant color usage', 'Eye-catching design', 'Extreme typography', 'Exceptional design'] }
      ]
    };
  }
};
</script>

<template>
  <main>
    <!-- Header Section -->
    <header class="header-section container-fluid">
  <div class="row">
    <div class="col-lg-6 d-flex flex-column justify-content-center align-items-start p-5">
      <p class="experience-text">17 YEARS OF EXPERIENCE</p>
      <h1>We Are a Web Design <span class="highlight">Agency</span></h1>
      <p>Far Far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean. Separated they live in Bookmarksgrove.</p>
      <button class="btn btn-dark btn-lg">Read More</button>
      <div class="social-icons mt-4">
        <a href="#">Facebook</a>
        <a href="#">Instagram</a>
        <a href="#">Twitter</a>
        <a href="#">YouTube</a>
      </div>
    </div>
    <div class="col-lg-6 p-0">
     
        <img src="/public/img/images/Group-36-2x.png" alt="Header Image" class="img-fluid" />
     
    </div>
  </div>
</header>


    <!-- Services Section -->
    <section class="services-section text-center m my-5">
  <div class="container d-flex align-items-center">
    <!-- Testo a sinistra -->
    <div class="text-container  col-md-6">
      <h1>We Are Here To Make Your <span class="highlight">Website</span> Look More <span class="highlight">Elegant</span> And Stylish!</h1>
      <button class="btn btn-success view-all-btn mt-4">View All</button>
    </div>

    <!-- Carte a destra -->
    <div class="cards-container row col-md-6">
      <div class="col-md-6 col-lg-6 mb-4" v-for="service in services" :key="service.title">
        <div class="card service-card h-100">
          <div class="card-body d-flex flex-column">
            <div class="service-icon mb-3"><!-- Placeholder per l'icona --></div>
            <h5 class="card-title">{{ service.title }}</h5>
            <p class="card-text">{{ service.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>




    <!-- Mission Section -->
    <section class="mission-section container my-5">
  <div class="row">
    <div class="col-md-6">    
      <img src="/public/img/images/businesswoman-analysing-document-P8WSNMC-1024x820.jpg" alt="Mission Image" class="img-fluid main-image" />
    </div>
    <div class="col-md-6 d-flex flex-column justify-content-center p-5">
      <h2>Learn more about our <span class="highlight">missions</span></h2>
      <p>Far Far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean. Separated they live in Bookmarksgrove.</p>
      <button class="btn btn-success">Read More</button>
    </div>
  </div>
</section>



    <!-- Recent Projects Section -->
    <section class="recent-projects py-5">
  <div class="container">
    <div class="row">
    
      <div class="col-lg-6 d-flex flex-column justify-content-center">
        <h2>Our recent <span class="highlight">web designs</span> & some examples of past <span class="highlight">projects</span></h2>
      </div>
     
      <div class="col-lg-6">
        <p>Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean. Separated they live in Bookmarksgrove.</p>
      </div>
    </div>

    <div class="row mt-4 projects-grid">
      <div class="col-md-3 project-card" v-for="project in projects" :key="project.alt">
        <img :src="project.src" :alt="project.alt" class="img-fluid" />
      </div>
    </div>
  </div>
</section>

    <!-- Stats Section -->
    <section class="stats-section py-5">
  <div class="container">
    <div class="row align-items-center">
    
      <div class="col-lg-6 stats-bg p-5 text-white">
        <h2 class="display-4">280</h2>
        <p>PROJECTS</p>
        <h2 class="display-4">+3,500</h2>
        <p>USERS' COMMENTS</p>
        <h2 class="display-4">100%</h2>
        <p>HAPPY CLIENTS</p>
      </div>

     
      <div class="col-lg-6 p-5">
        <h2>We <span class="highlight">Love</span> What We Do</h2>
        <p>Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts...</p>
        <ul>
          <li><i class="check-icon"></i> Far far away, behind the word mountains</li>
          <li><i class="check-icon"></i> Large language ocean</li>
          <li><i class="check-icon"></i> Far from the countries Vokalia and Consonantia</li>
        </ul>
      </div>
    </div>
  </div>
</section>


    <!-- Pricing Section -->
    <section class="pricing-section py-5">
      <div class="container">
        <h2 class="text-center">With <span class="highlight">Live Chat</span> 24/7 Support</h2>
        <div class="row">
          <div class="pricing-card" v-for="price in pricing" :key="price.title">
            <div class="card">
              <div class="card-header">
                <h3 class="card-title">{{ price.title }}</h3>
              </div>
              <div class="card-body">
                <h4 class="price">{{ price.cost }}</h4>
                <ul>
                  <li v-for="feature in price.features" :key="feature">{{ feature }}</li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Testimonial Section -->
    <section class="testimonial-section">
      <div class="content text-center">
        <p class="quote">
          "When it comes to barbequing, there are two main schools of thought for the techniques that you can use. Freshly scrambled eggs with applewood smoked bacon - are amazing!"
        </p>
        <img class="testimonial-img" src="/img/images/businesswoman-analysing-document-P8WSNMC-1024x820.jpg" alt="">
        <h4 class="testimonial-author">LISSA DURBIN</h4>
        <p>Client</p>
      </div>
    </section>

    <!-- Blog Section -->
     <section class="blog-section py-5">
    <div class="container">
      <h2 class="text-center">Latest News & Our Blog</h2>
      <div class="row mt-4">
        <div class="col-md-4 blog-item-wrapper" v-for="post in blogPosts" :key="post.title" >
          <div class="card blog-card">
            <div class="image-container">
              <img :src="post.image" class="card-img-top blog-image" :alt="post.title">
            </div>
            <div class="card-body blog-body">
              <span class="blog-date">{{ post.date }}</span>
              <h5 class="card-title">{{ post.title }}</h5>
              <p class="card-text">{{ post.excerpt }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

    <!-- Contact Section -->
    <section class="contact-section py-5 text-center">
  <div class="container">
    <div class="row justify-content-center">
      <!-- Start a New Project -->
      <div class="col-lg-6">
        <div class="card contact-card dark-card">
          <div class="card-body">
            <p class="small-text">Are You Ready?</p>
            <h2 class="card-title">Start a New Project</h2>
            <div class="input-group mt-4">
              <input type="email" class="form-control" placeholder="Enter Your Email Address" aria-label="Email">
              <button class="btn btn-dark">SUBMIT</button>
            </div>
          </div>
        </div>
      </div>

      <!-- Let's Talk About Work -->
      <div class="col-lg-6">
        <div class="card contact-card green-card">
          <div class="card-body">
            <p class="small-text">What Are You Waiting for?</p>
            <h2 class="card-title">Let's Talk About Work</h2>
            <button class="btn btn-dark mt-4">START NOW</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

  </main>
</template>



<style scoped>
.header-section {
  background-color: #f8f9fa;
  padding: 50px 0;
  position: relative;
}

.experience-text {
  color: #1fcf95;
  font-size: 1rem;
  letter-spacing: 2px;
  text-transform: uppercase;
  font-weight: 600;
}

h1 {
  font-size: 3.5rem;
  font-weight: 700;
  line-height: 1.2;
  margin-bottom: 20px;
}

.highlight {
  color: #1fcf95;
  font-weight: 700;
}

p {
  font-size: 1rem;
  color: #6c757d;
  margin-bottom: 30px;
}

.btn-lg {
  padding: 15px 40px;
  font-size: 1.2rem;
}


.social-icons {
  margin-top: 20px;
}

.social-icons a {
  color: #000;
  font-size: 1rem;
  margin-right: 20px;
  text-decoration: none;
  transition: color 0.3s ease;
}

.social-icons a:hover {
  color: #1fcf95;
}
.services-section .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.text-container {
  text-align: left;
}

.cards-container {
  display: flex;
  flex-wrap: wrap;
}

.card {
  height: 100%; 
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  margin: 10px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  transition: transform 0.3s ease, box-shadow 0.3s ease, background-color 0.3s ease; /* Aggiungi transizioni */
}

/* Hover effetto */
.card:hover {
  transform: translateY(-5px); 
  background-color: #1fcf95;
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.2);
}

.view-all-btn {
  margin-top: 20px;
}

.main-image {
  position: relative;
  z-index: 2;
  border-radius: 10px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
}

h2 {
  font-size: 2.5rem;
  font-weight: bold;
}

.highlight {
  color: #1fcf95;
  font-weight: bold;
}

button.btn-success {
  background-color: #1fcf95;
  border: none;
  width: 120px;
  padding: 10px 20px;
  border-radius: 30px;
  box-shadow: 0 4px 15px rgba(31, 207, 149, 0.3);
}

button.btn-success:hover {
  background-color: #17a589;
  box-shadow: 0 6px 20px rgba(31, 207, 149, 0.5);
}

.recent-projects h2 {
  font-size: 2.5rem;
  font-weight: bold;
  line-height: 1.2;
  margin-bottom: 20px;
}

.recent-projects .highlight {
  color: #1fcf95;
}

.recent-projects p {
  font-size: 1rem;
  color: #6c757d;
}

.project-card img {
  width: 100%;
  height: auto;
  border-radius: 8px;
  transition: transform 0.3s ease;
}

.project-card:hover img {
  transform: scale(1.05);
}

.stats-section {
  position: relative;
  background-color: #f8f9fa;
}

.stats-bg {
  background-color: #1fcf95;
  border-radius: 15px;
  color: #fff;
  padding: 40px;
}

h2 .highlight {
  color: #1fcf95;
}

.check-icon {
  color: #1fcf95;
  margin-right: 10px;
}

ul {
  list-style: none;
  padding: 0;
}

ul li {
  font-size: 1.2rem;
  margin-bottom: 10px;
}

ul li::before {
  content: '\2713';
  color: #1fcf95;
  font-weight: bold;
  margin-right: 10px;
}


.pricing-section .pricing-card {
  display: inline-block;
  width: 30%;
  margin-bottom: 20px;
}

.pricing-section .card {
  border: none;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.pricing-section .card-header {
  background-color: #343a40;
  color: white;
}

.pricing-section .price {
  font-size: 1.5rem;
  margin-top: 10px;
}

.testimonial-section {
  background-image: url('/public/img/images/four-businesspeople-in-a-boardroom-with-paperwork-PC4V8H4.jpg');
  background-size: cover;
  background-position: center;
  position: relative;
  padding: 100px 0;
 
  
}

.testimonial-section::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  z-index: 1;
  

}

.testimonial-img {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  margin: 20px auto;
  display: block;
}

.quote {
  font-size: 1.5rem;
  color: #fff;
  margin-bottom: 20px;
}

.testimonial-author {
  color: #20c997;
  font-weight: bold;
  font-size: 1.2rem;
}

.blog-section {
  position: relative;
  z-index: 1;
}

.blog-item-wrapper {
  position: relative;
  z-index: 2;
  margin-bottom: 40px;
}

.blog-card {
  position: relative;
  background-color: #fff;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease-in-out;
  z-index: 3;
  margin-top: -30px; 
}

.blog-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.15);
}

.blog-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
  transition: transform 0.3s ease;
}

.blog-body {
  padding: 20px;
  background-color: #fff;
}

.blog-card:hover .blog-image {
  transform: scale(1.05);
}

.image-container {
  position: relative;
  overflow: hidden;
  border-radius: 8px;
}

.blog-date {
  font-size: 0.85rem;
  color: #999;
  display: block;
  margin-bottom: 10px;
}

.card-title {
  font-size: 1.2rem;
  font-weight: bold;
  margin-bottom: 10px;
}

.card-text {
  font-size: 1rem;
  color: #666;
}

.contact-section {
  background-color: #f8f9fa;
  padding: 80px 0;
}

.contact-card {
  border-radius: 20px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
  padding: 40px;
  text-align: center;
}

.dark-card {
  background-color: #222;
  color: #fff;
}

.green-card {
  background: linear-gradient(90deg, rgba(43,194,152,1) 0%, rgba(72,225,173,1) 100%);
  color: #fff;
}

.small-text {
  font-size: 14px;
  color: #bbb;
}

.card-title {
  font-size: 2rem;
  font-weight: 700;
}

.input-group {
  display: flex;
  justify-content: center;
  align-items: center;
}

.input-group .btn {
  border-radius: 50px;
  padding: 15px 30px;
  font-size: 1rem;
}

.green-card .btn {
  background-color: #222;
  color: #fff;
}

</style>
