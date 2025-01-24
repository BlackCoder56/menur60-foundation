<template>
  <footer class="footer bg-dark text-light py-4">
    <div class="container">
      <div class="row text-center text-md-start">
        <!-- Join Us -->
        <div class="col-md-4 col-12 mb-3">
          <h5 class="fw-bold text-success">Join Us</h5>
          <p>Be a part of our community and help make a difference.</p>
          <a href="#" class="btn btn-outline-success btn-sm">Sign Up</a>
        </div>

        <!-- Follow Us -->
        <div class="col-md-4 col-12 mb-3">
          <h5 class="fw-bold text-success">Follow Us</h5>
          <ul class="list-unstyled">
            <li>
              <a href="#" class="text-light">
                <i class="bi bi-facebook mx-1 text-success"></i> Facebook
              </a>
            </li>
            <li>
              <a href="#" class="text-light">
                <i class="bi bi-twitter-x mx-1 text-success"></i> Twitter
              </a>
            </li>
            <li>
              <a href="#" class="text-light">
                <i class="bi bi-instagram mx-1 text-success"></i> Instagram
              </a>
            </li>
            <li>
              <a href="#" class="text-light">
                <i class="bi bi-linkedin mx-1 text-success"></i> LinkedIn
              </a>
            </li>
          </ul>
        </div>

        <!-- Operation Areas -->
        <div class="col-md-4 col-12 mb-3">
          <h5 class="fw-bold text-success">Areas of Operation</h5>
          <ul class="list-unstyled">
            <li>Soroti</li>
            <li>Lira</li>
            <li>Gulu</li>
            <li>Mbale</li>
            <li>Kitgum</li>
          </ul>
        </div>
      </div>

      <!-- Bottom Bar -->
      <div class="d-flex justify-content-between align-items-center mt-4">
        <small>&copy; 2025 All Rights Reserved</small>
        <a href="https://github.com/yourgithub" class="text-success" target="_blank">
          <i class="bi bi-github"></i> GitHub
        </a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Menur60Footer",
};
</script>

<style scoped>
.footer {
  background: #2b2b2b;
}
.footer a {
  text-decoration: none;
}
.footer a:hover {
  text-decoration: underline;
}
</style>
