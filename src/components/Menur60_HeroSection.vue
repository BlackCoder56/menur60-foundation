<template>
    <section class="hero bg-light">
      <div class="container">
        <div class="row align-items-center text-center text-md-start">
          <!-- Left Content -->
          <div class="col-md-6 text-container">
            <h1 class="display-4 fw-bold text-success mb-3 animated-title">
              Empowering Communities, Changing Lives
            </h1>
            <p class="lead text-muted mb-4">
              Join us in making a difference by supporting sustainable development initiatives across the globe. Together, we can create a brighter future.
            </p>
            <a href="#about" class="btn btn-success btn-lg px-4">
              Learn More
            </a>
          </div>
  
          <!-- Right Image -->
          <div class="col-md-6 d-none d-md-block animated-image">
            <img
              :src="require('@/assets/img/hero.jpeg')"
              alt="Hero Image"
              class="img-fluid rounded shadow"
            />
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: "HeroSection",
  };
  </script>
  
  <style scoped>
  /* Hero Section Styling */
  .hero {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh; /* Full viewport height */
    background: linear-gradient(to bottom right, #f5f5f5, rgba(255, 255, 255, 0.9));
    position: relative;
  }
  
  .animated-title {
    opacity: 0;
    animation: fadeIn 2s ease-out forwards;
  }
  
  /* Image fade-in animation for mobile */
  .animated-image img {
    opacity: 0;
    animation: fadeIn 3s ease-out forwards;
  }
  
  /* Slide-in animation for larger screens */
  @media (min-width: 768px) {
    .animated-image {
      transform: translateX(100%);
      animation: slideIn 2s ease-out forwards;
    }
  }
  
  /* Fade-in keyframes */
  @keyframes fadeIn {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }
  
  /* Slide-in keyframes */
  @keyframes slideIn {
    0% {
      transform: translateX(100%);
    }
    100% {
      transform: translateX(0);
    }
  }
  
  .hero h1 {
    line-height: 1.2;
  }
  
  .hero img {
    max-width: 100%;
    height: auto;
  }
  
  /* Background image for mobile view */
  @media (max-width: 768px) {
     /* Add a semi-transparent background for text on mobile */
    .text-container {
        background: rgba(255, 255, 255, 0.8); /* Semi-transparent white */
        padding: 1rem;
        border-radius: 8px; /* Rounded corners */
    }
    .hero {
      background-image: url("@/assets/img/hero.jpeg");
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      padding: 2rem; /* Add padding for better readability */
    }
  
    .hero img {
      display: none; /* Hide inline image on mobile */
    }
  }
  </style>
  