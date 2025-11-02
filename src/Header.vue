<template>
  <nav
    class="navbar navbar-expand-lg navbar-dark position-sticky top-0 header-container"
  >
    <div class="container-fluid">
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div
        class="collapse navbar-collapse header-margin"
        id="navbarSupportedContent"
      >
        <ul
          class="navbar-nav w-100 d-flex justify-content-between align-items-center text-light"
        >
          <li class="nav-item">
            <a class="nav-link text-light" href="#about">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-light" href="#works">Works</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-light" href="#experience"
              >Education & Experience</a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link text-light" href="#skills">Skills</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-light" href="#contact">Contact</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { onMounted, onBeforeUnmount } from "vue";

onMounted(() => {
  const toggler = document.querySelector(".navbar-toggler");
  const collapseEl = document.getElementById("navbarSupportedContent");
  const links = document.querySelectorAll(".navbar-nav .nav-link");

  const handler = () => {
    if (!toggler || !collapseEl) return;
    // If toggler is visible (mobile) and collapse is open, click toggler to close
    const togglerStyle = window.getComputedStyle(toggler);
    if (
      togglerStyle.display !== "none" &&
      collapseEl.classList.contains("show")
    ) {
      toggler.click();
    }
  };

  links.forEach((l) => l.addEventListener("click", handler));
  // store for cleanup
  window.__header_nav_cleanup = { links: Array.from(links), handler };
});

onBeforeUnmount(() => {
  const info = window.__header_nav_cleanup;
  if (info) {
    info.links.forEach((l) => l.removeEventListener("click", info.handler));
    delete window.__header_nav_cleanup;
  }
});
</script>

<style scoped>
@media (min-width: 992px) {
  .header-margin {
    margin: 0 15rem;
  }
}

.header-container {
  background-color: #33020a;
  z-index: 100;
}
</style>
