<template>
  <section class="projects-page bg-light py-5">
    <div class="container">
      <!-- Heading -->
      <div class="text-center mb-5">
        <h1 class="fw-bold text-success">Projects</h1>
        <p class="text-muted">Discover some of the impactful initiatives we have undertaken.</p>
      </div>

      <!-- Project Cards -->
      <div class="row">
        <!-- Project 1 -->
        <div class="col-md-6 col-lg-4 mb-4">
          <div class="project-card bg-white rounded shadow-sm p-4 fade-in">
            <img 
              :src="require('@/assets/img/projects/project1.jpg')"
              alt="Project 1" 
              class="img-fluid rounded mb-3">
            <h5 class="fw-bold text-success">Reforestation Drive</h5>
            <p>Empowering communities to plant and nurture trees for a sustainable future.</p>
            <a href="#" class="btn btn-outline-success btn-sm">Read More</a>
          </div>
        </div>

        <!-- Project 2 -->
        <div class="col-md-6 col-lg-4 mb-4">
          <div class="project-card bg-white rounded shadow-sm p-4 fade-in">
            <img 
               :src="require('@/assets/img/projects/project2.jpg')"
              alt="Project 2" 
              class="img-fluid rounded mb-3">
            <h5 class="fw-bold text-success">Clean Energy Workshops</h5>
            <p>Educating communities about solar and wind energy to reduce carbon footprints.</p>
            <a href="#" class="btn btn-outline-success btn-sm">Read More</a>
          </div>
        </div>

        <!-- Project 3 -->
        <div class="col-md-6 col-lg-4 mb-4">
          <div class="project-card bg-white rounded shadow-sm p-4 fade-in">
            <img 
               :src="require('@/assets/img/projects/project3.jpg')"
              alt="Project 3" 
              class="img-fluid rounded mb-3">
            <h5 class="fw-bold text-success">Youth Climate Action</h5>
            <p>Engaging young minds to lead climate initiatives and drive innovation.</p>
            <a href="#" class="btn btn-outline-success btn-sm">Read More</a>
          </div>
        </div>

        <!-- Project 4 -->
        <div class="col-md-6 col-lg-4 mb-4">
          <div class="project-card bg-white rounded shadow-sm p-4 fade-in">
            <img 
               :src="require('@/assets/img/projects/project4.jpg')"
              alt="Project 4" 
              class="img-fluid rounded mb-3">
            <h5 class="fw-bold text-success">Waste Management Program</h5>
            <p>Turning waste into resources through recycling and composting initiatives.</p>
            <a href="#" class="btn btn-outline-success btn-sm">Read More</a>
          </div>
        </div>

        <!-- Project 5 -->
        <div class="col-md-6 col-lg-4 mb-4">
          <div class="project-card bg-white rounded shadow-sm p-4 fade-in">
            <img 
            :src="require('@/assets/img/projects/project5.jpg')" 
              alt="Project 5" 
              class="img-fluid rounded mb-3">
            <h5 class="fw-bold text-success">Water Conservation Campaign</h5>
            <p>Promoting efficient water usage and building rainwater harvesting systems.</p>
            <a href="#" class="btn btn-outline-success btn-sm">Read More</a>
          </div>
        </div>

        <!-- Project 6 -->
        <div class="col-md-6 col-lg-4 mb-4">
          <div class="project-card bg-white rounded shadow-sm p-4 fade-in">
            <img 
               :src="require('@/assets/img/projects/project6.jpg')"
              alt="Project 6" 
              class="img-fluid rounded mb-3">
            <h5 class="fw-bold text-success">Community Farming Initiative</h5>
            <p>Empowering local farmers with tools, training, and sustainable practices.</p>
            <a href="#" class="btn btn-outline-success btn-sm">Read More</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ProjectsPage",
};
</script>

<style scoped>
.projects-page {
  background: linear-gradient(to bottom, #E3FDFD, #D4F8E8, #FFEFD6);
  animation: fadeInBg 2s ease-in-out;
  height: 95vh;
}

.project-card {
  transition: transform 0.3s, box-shadow 0.3s;
  animation: fadeIn 1.5s ease-in-out forwards;
  opacity: 0;
  box-shadow: 20px 10px #000; 
}

.project-card:hover {
  transform: translateY(-5px) scale(1.02);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
}

.fade-in {
  animation: fadeIn 1.5s ease-in-out forwards;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes fadeInBg {
  0% {
    background: #030303;
  }
  100% {
    background: linear-gradient(to bottom, #E3FDFD, #D4F8E8, #FFEFD6);
  }
}

@media (max-width: 768px) {
  .project-card {
    margin-bottom: 1.5rem;
  }
}
</style>
