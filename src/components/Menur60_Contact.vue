<template>
  <section class="contact-page bg-light py-5">
    <div class="container">
      <!-- Heading -->
      <div class="text-center mb-5">
        <h1 class="fw-bold text-success">Contact Us</h1>
        <p class="text-muted">We would love to hear from you. Get in touch with us!</p>
      </div>

      <div class="row">
        <!-- Contact Form -->
        <div class="col-lg-7 mb-4">
          <div class="bg-white rounded shadow-sm p-4">
            <h5 class="fw-bold text-success mb-4">Send Us a Message</h5>
            <form>
              <div class="mb-3">
                <label for="name" class="form-label">Your Name</label>
                <input type="text" class="form-control" id="name" placeholder="Enter your name">
              </div>
              <div class="mb-3">
                <label for="email" class="form-label">Email Address</label>
                <input type="email" class="form-control" id="email" placeholder="Enter your email">
              </div>
              <div class="mb-3">
                <label for="message" class="form-label">Message</label>
                <textarea class="form-control" id="message" rows="5" placeholder="Write your message here..."></textarea>
              </div>
              <button type="submit" class="btn btn-success">Send Message</button>
            </form>
          </div>
        </div>

        <!-- Contact Details -->
        <div class="col-lg-5">
          <div class="bg-white rounded shadow-sm p-4">
            <h5 class="fw-bold text-success mb-4">Get in Touch</h5>
            <p class="mb-2"><i class="bi bi-geo-alt-fill text-success"></i> 123 Green Street, Eco City</p>
            <p class="mb-2"><i class="bi bi-telephone-fill text-success"></i> +1 (234) 567-890</p>
            <p class="mb-2"><i class="bi bi-envelope-fill text-success"></i> info@example.com</p>
            <h6 class="fw-bold mt-4">Follow Us</h6>
            <div class="d-flex gap-3">
              <a href="#" class="text-success fs-4"><i class="bi bi-facebook"></i></a>
              <a href="#" class="text-success fs-4"><i class="bi bi-twitter"></i></a>
              <a href="#" class="text-success fs-4"><i class="bi bi-instagram"></i></a>
              <a href="#" class="text-success fs-4"><i class="bi bi-linkedin"></i></a>
            </div>
          </div>
        </div>
      </div>

      <!-- Google Map Embed -->
      <div class="mt-5">
        <div class="bg-white rounded shadow-sm p-4">
          <h5 class="fw-bold text-success mb-4">Find Us Here</h5>
          <iframe 
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d63808.253323345816!2d33.57533344508558!3d1.7223189049916934!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x1779b9ffc3d63557%3A0x7923a22894bc2ef9!2sSoroti!5e0!3m2!1sen!2sug!4v1737706042996!5m2!1sen!2sug"
            width="100%" 
            height="400" 
            style="border:0;" 
            allowfullscreen="" 
            loading="lazy" 
            referrerpolicy="no-referrer-when-downgrade">
          </iframe>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContactPage",
};
</script>

<style scoped>
.contact-page {
  background: linear-gradient(to bottom, #E3FDFD, #D4F8E8, #FFEFD6);
  animation: gradientShift 10s ease infinite;
}

@keyframes gradientShift {
  0%, 100% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
}

.bg-white {
  animation: fadeIn 1.5s ease-in-out forwards;
  opacity: 0;
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

@media (max-width: 768px) {
  .text-center {
    margin-bottom: 1.5rem;
  }

  .bg-white {
    margin-bottom: 1.5rem;
  }
}
</style>
