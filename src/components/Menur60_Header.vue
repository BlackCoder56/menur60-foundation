<template>
  <header>
    <nav class="navbar navbar-expand-lg navbar-dark bg-success shadow fixed-top">
      <div class="container">
        <!-- Logo and Brand -->
        <a class="navbar-brand d-flex align-items-center gap-2" href="#">
          <div
            class="rounded-circle bg-warning text-center text-dark fw-bold d-flex justify-content-center align-items-center"
            style="width: 40px; height: 40px;"
          >
            M60
          </div>
          <span>Menur 60 Foundation</span>
        </a>

        <!-- Hamburger Menu -->
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <!-- Navigation Links -->
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto text-center">
            <li class="nav-item">
              <a
                class="nav-link"
                href="#home"
                :class="{ active: activeLink === '#home' }"
                @click="setActiveLink('#home')"
              >Home</a>
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                href="#about"
                :class="{ active: activeLink === '#about' }"
                @click="setActiveLink('#about')"
              >About</a>
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                href="#projects"
                :class="{ active: activeLink === '#projects' }"
                @click="setActiveLink('#projects')"
              >Projects</a>
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                href="#services"
                :class="{ active: activeLink === '#services' }"
                @click="setActiveLink('#services')"
              >Services</a>
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                href="#contact"
                :class="{ active: activeLink === '#contact' }"
                @click="setActiveLink('#contact')"
              >Contact</a>
            </li>
          </ul>

          <!-- Twitter Icon -->
          <div class="mt-3 text-center">
            <a href="https://twitter.com" target="_blank" class="text-white">
              <i class="bi bi-twitter fs-4"></i>
            </a>
          </div>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: "HeaderNavbar",
  data() {
    return {
      activeLink: "#home", // Default active link
    };
  },
  methods: {
    setActiveLink(link) {
      this.activeLink = link;
    },
  },
};
</script>

<style scoped>
/* Additional styling for the logo */
.navbar-brand .rounded-circle {
  font-size: 1.1rem;
}

/* Add hover and active effects */
.nav-link:hover,
.nav-link.active {
  color: #ffd700 !important; /* Golden color for text */
  background-color: rgba(255, 255, 255, 0.2); /* Faded white background */
  border-radius: 5px;
  transition: background-color 0.3s ease, color 0.3s ease;
}

/* Twitter icon styling */
.bi-twitter {
  transition: transform 0.3s ease;
}
.bi-twitter:hover {
  transform: scale(1.2);
  color: #1da1f2; /* Twitter blue */
}
</style>
