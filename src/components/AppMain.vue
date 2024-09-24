<template>
  <main>
    <!-- Header Section -->
    <header class="header-section container-fluid p-0">
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
    <section class="services-section text-center my-5">
  <div class="container">
    <h2>We Are Here To Make Your <span class="highlight">Website</span> Look More <span class="highlight">Elegant</span> And Stylish!</h2>
    <div class="row mt-4">
      <div class="col-md-6 col-lg-3 mb-4" v-for="service in services" :key="service.title">
        <div class="card service-card">
          <div class="card-body">
            <div class="service-icon"><!-- Placeholder for icon if needed --></div>
            <h5 class="card-title">{{ service.title }}</h5>
            <p class="card-text">{{ service.description }}</p>
          </div>
        </div>
      </div>
    </div>
    <button class="btn btn-success view-all-btn">View All</button>
  </div>
</section>


    <!-- Mission Section -->
    <section class="mission-section container my-5">
      <div class="row">
        <div class="col-md-6">
          <img src="/public/img/images/businesswoman-analysing-document-P8WSNMC-1024x820.jpg" alt="Mission Image" class="img-fluid" />
        </div>
        <div class="col-md-6">
          <h2>Learn more about our <span class="highlight">missions</span></h2>
          <p>Far Far away, behind the word mountains, far from the countries Vokalia and Consonantia...</p>
          <button class="btn btn-success">Learn More</button>
        </div>
      </div>
    </section>

    <!-- Recent Projects Section -->
    <section class="recent-projects py-5">
      <div class="container">
        <h2 class="text-center">Our Recent <span class="highlight">Web Designs</span> & Some Examples of Past <span class="highlight">Projects</span></h2>
        <div class="projects-grid">
          <div class="project-card" v-for="project in projects" :key="project.alt">
            <img :src="project.src" :alt="project.alt" class="img-fluid" />
          </div>
        </div>
      </div>
    </section>

    <!-- Stats Section -->
    <section class="stats-section py-5 bg-light">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-md-4 text-center">
            <h2>280</h2>
            <p>PROJECTS</p>
          </div>
          <div class="col-md-4 text-center">
            <h2>+3,500</h2>
            <p>USERS' COMMENTS</p>
          </div>
          <div class="col-md-4 text-center">
            <h2>100%</h2>
            <p>HAPPY CLIENTS</p>
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

.services-section {
  padding: 60px 0;
  text-align: left;
}

h2 {
  font-size: 2.5rem;
  font-weight: 700;
  margin-bottom: 30px;
}

.highlight {
  color: #1fcf95;
  font-weight: 700;
}

.card-container {
  display: flex;
  justify-content: space-between;
}

.service-card {
  background-color: #fff;
  border-radius: 12px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  padding: 20px;
  transition: transform 0.3s ease-in-out;
  height: 100%;
}

.service-card:hover {
  transform: translateY(-5px);
}

.card-body {
  padding: 30px 20px;
  text-align: center;
}

.card-title {
  font-size: 1.25rem;
  font-weight: 600;
  margin-top: 15px;
}

.card-text {
  font-size: 1rem;
  color: #6c757d;
  margin-top: 10px;
}

.service-icon {
  width: 50px;
  height: 50px;
  background-color: transparent;
  border: 2px solid #1fcf95;
  border-radius: 8px;
  margin: 0 auto 20px;
}

.view-all-btn {
  background: linear-gradient(90deg, rgba(43, 194, 152, 1) 0%, rgba(72, 225, 173, 1) 100%);
  border: none;
  border-radius: 50px;
  padding: 10px 30px;
  font-size: 1rem;
  color: #fff;
  transition: background 0.3s ease-in-out;
  box-shadow: 0 5px 15px rgba(31, 207, 149, 0.3);
}

.view-all-btn:hover {
  background: rgba(31, 207, 149, 1);
  box-shadow: 0 8px 25px rgba(31, 207, 149, 0.5);
}


.mission-section img {
  max-width: 100%;
  height: auto;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
}

.projects-grid img {
  width: 100%;
  height: auto;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.stats-section {
  background-color: #e9ecef;
  padding: 50px 0;
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
  margin-top: -30px; /* Overlap with image */
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

.input-group .form-control {
  background-color: rgba(255, 255, 255, 0.1);
  border: none;
  border-radius: 50px;
  color: #fff;
  padding: 15px;
  max-width: 300px;
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
