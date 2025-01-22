<template>
  <section class="about-page bg-light py-5">
    <div class="container">
        <!-- Page Heading -->
        <h1 class="text-center fw-bold text-success mb-5">About Us</h1>
      <!-- Top Picture (Visible on Desktop Only) -->
      <div class="top-image d-none d-md-block mb-4">
        <img 
          :src="require('@/assets/img/about-us.jpg')" 
          alt="About Us Image" 
          class="img-fluid rounded shadow">
      </div>

      <!-- About Us Content -->
      <div class="row text-center text-md-start">
        <!-- About Us Section -->
        <div class="col-md-6 mb-4">
          <div class="content-box p-4 bg-white rounded shadow-sm fade-in">
            <h3 class="fw-bold text-success mb-3">About Menur60<sup>0</sup></h3>
            <p>
              We aim to create a resilient future by promoting regenerative practices, community empowerment, and environmental stewardship. 
              By fostering collaboration among communities and integrating innovative solutions, we work to address environmental challenges effectively. 
              Our commitment is to provide impactful initiatives that inspire sustainable change and enhance lives for the long term.
            </p>
          </div>
        </div>

        <!-- Our Vision Section -->
        <div class="col-md-6 mb-4">
          <div class="content-box p-4 bg-white rounded shadow-sm fade-in">
            <h3 class="fw-bold text-success mb-3">Our Vision</h3>
            <p>
              "A sustainable world where empowered women and youth lead the transformation of agriculture, create resilient livelihoods, 
              and champion climate action for thriving communities and a balanced ecosystem." We envision a future where communities flourish through 
              innovative practices, ensuring equity and environmental health. Together, we strive to create an impactful legacy of sustainability and harmony.
            </p>
          </div>
        </div>

        <!-- Our Values Section -->
        <div class="col-md-6 mb-4">
          <div class="content-box p-4 bg-white rounded shadow-sm fade-in">
            <h3 class="fw-bold text-success mb-3">Our Values</h3>
            <p>
              Sustainability, Innovation, Women and Youth Leadership, Inclusivity, Collaboration, Resilience, Environmental Stewardship, Empowerment, 
              and Accountability. These core values guide our mission to drive impactful changes across communities. Our unwavering dedication to these principles 
              fuels our pursuit of transformative and sustainable solutions for the betterment of society and the environment.
            </p>
          </div>
        </div>

        <!-- Empowerment Section -->
        <div class="col-md-6 mb-4">
          <div class="content-box p-4 bg-white rounded shadow-sm fade-in">
            <h3 class="fw-bold text-success mb-3">Empowerment</h3>
            <p>
              We equip individuals and communities with the knowledge, tools, and skills needed to improve livelihoods and make informed decisions 
              for a sustainable future. Through our hands-on programs, we aim to inspire confidence and independence, enabling participants to thrive 
              in their efforts to build a better tomorrow. Together, we foster a culture of self-reliance and proactive engagement.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AboutPage",
};
</script>

<style scoped>
.about-page {
  background: linear-gradient(to bottom, #E3FDFD, #D4F8E8, #FFEFD6);
}

.top-image {
  width: 100%;
  height: auto;
}

img{
    position: relative;
    width: 100%;
    height: 30vh;
}

.content-box {
  border: 1px solid #e0e0e0;
  transition: transform 0.3s, box-shadow 0.3s;
  animation: fadeIn 1s ease-in-out;
  opacity: 0;
}

.content-box:hover {
  transform: translateY(-5px) scale(1.02);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
}

.fade-in {
  animation: fadeIn 1.5s ease-in-out forwards;
}

/* Fade-in animation */
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

@media (max-width: 768px) {
  .top-image {
    display: none;
  }

  .content-box {
    margin-bottom: 1.5rem;
  }
}
</style>
