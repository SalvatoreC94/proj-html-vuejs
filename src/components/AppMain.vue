<template>
  <main>
    <!-- Header Section -->
    <header class="header-section container-fluid p-0">
      <div class="row">
        <div class="col-lg-6 d-flex flex-column justify-content-center align-items-start p-5">
          <h1>We Are a Web Design Agency</h1>
          <p>
            Far Far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.
          </p>
          <button class="btn btn-dark">Read More</button>
        </div>
        <div class="col-lg-6 p-0">
          <img src="" alt="Header Image" class="img-fluid w-100" />
        </div>
      </div>
    </header>

    <!-- Services Section -->
    <section class="services-section container my-5">
      <div class="row text-center mb-4">
        <div class="col">
          <h2>We Are Here To Make Your Website Look More Elegant And Stylish!</h2>
          <button class="btn btn-success mt-3">View All</button>
        </div>
      </div>
      <div class="row">
        <div class="col-md-6 col-lg-3 mb-4">
          <div class="card service-card h-100">
            <div class="card-body text-center">
              <h5 class="card-title">Speed Optimization</h5>
              <p class="card-text">Far Far away, behind the word mountains...</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg-3 mb-4">
          <div class="card service-card h-100">
            <div class="card-body text-center">
              <h5 class="card-title">Cloud Solutions</h5>
              <p class="card-text">Far Far away, behind the word mountains...</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg-3 mb-4">
          <div class="card service-card h-100">
            <div class="card-body text-center">
              <h5 class="card-title">Website Design</h5>
              <p class="card-text">Far Far away, behind the word mountains...</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg-3 mb-4">
          <div class="card service-card h-100">
            <div class="card-body text-center">
              <h5 class="card-title">Online Marketing</h5>
              <p class="card-text">Far Far away, behind the word mountains...</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Mission Section -->
    <section class="mission-section container my-5">
      <div class="row align-items-center">
        <div class="col-md-6">
          <img src="" alt="Mission Image" class="img-fluid" />
        </div>
        <div class="col-md-6">
          <h2>Learn more about our missions</h2>
          <p>Far Far away, behind the word mountains, far from the countries Vokalia and Consonantia...</p>
          <button class="btn btn-success mt-3">Learn More</button>
        </div>
      </div>
    </section>

    <!-- Recent Projects Section -->
    <section class="projects-section container d-flex my-5">
      <h2 class="text-center">Our recent web designs & some examples of past projects</h2>
      <div class="row my-4">
        <div class="col-md-3 mb-4">
          <div class="card project-card h-100">
            <div class="card-body">
              <h5 class="card-title">Project 1</h5>
              <p class="card-text">Far far away, behind the word mountains...</p>
            </div>
          </div>
        </div>
        <div class="col-md-3 mb-4">
          <div class="card project-card h-100">
            <div class="card-body">
              <h5 class="card-title">Project 2</h5>
              <p class="card-text">Far far away, behind the word mountains...</p>
            </div>
          </div>
        </div>
        <div class="col-md-3 mb-4">
          <div class="card project-card h-100">
            <div class="card-body">
              <h5 class="card-title">Project 3</h5>
              <p class="card-text">Far far away, behind the word mountains...</p>
            </div>
          </div>
        </div>
        <div class="col-md-3 mb-4">
          <div class="card project-card h-100">
            <div class="card-body">
              <h5 class="card-title">Project 4</h5>
              <p class="card-text">Far far away, behind the word mountains...</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Testimonial Section -->
    <section class="testimonial-section d-flex justify-content-center align-items-center">
  <div class="content text-center">
    <p>When it comes to barbequing, there are two main schools of thought for the techniques that you can use. Freshly scrambled eggs with applewood smoked bacon - are amazing!</p>
    <img class="testimonial-img" src="/img/images/businesswoman-analysing-document-P8WSNMC-1024x820.jpg" alt="">

    <h4>Lissa Durbin</h4>
    <h6>Client</h6>
  </div>
</section>


    <!-- Blog Section -->
  </main>
</template>

<script>
export default {
  name: 'HomePage'
};
</script>

<style scoped>
.header-section {
  background-color: #f8f9fa;
  padding: 50px 0;
}

.services-section .card {
  border: none;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease-in-out;
}

.services-section .card:hover {
  transform: translateY(-5px);
}

.mission-section img {
  max-width: 100%;
  height: auto;
}

.projects-section .card {
  border: none;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease-in-out;
}

.projects-section .card:hover {
  transform: translateY(-5px);
}

.testimonial-section {
  position: relative;
  height: 500px; 
  color: #fff;
  background-image: url('img/images/four-businesspeople-in-a-boardroom-with-paperwork-PC4V8H4.jpg');
  background-size: cover;
  background-position: center;
  display: flex;
  
}

.testimonial-section::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 500px;
  background-color: rgba(0, 0, 0, 0.8); 
  z-index: 1;
}

.content {
  position: relative;
  z-index: 2; 
  text-align: center;
}
/* aggiustare border radius */
.testimonial-img{    
  width: 100px;
 border-radius: 100%;
}


</style>
