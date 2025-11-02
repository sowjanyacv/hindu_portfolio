<script setup>
import About from "./components/About.vue";
import Contact from "./components/Contact.vue";
import Experience from "./components/Experience.vue";
import Home from "./components/Home.vue";
import Skills from "./components/Skills.vue";
import Works from "./components/Works.vue";
import Header from "./Header.vue";
</script>

<template>
  <main class="main-container w-100 overflow-hidden">
    <Header />
    <Home />
    <About />
    <Works />
    <Experience />
    <Skills />
    <Contact />
    <footer class="site-footer text-center text-white py-4">
      <div class="container">
        <p class="mb-1 small">
          Designed and developed using Vue.js by
          <a
            class="footer-link"
            href="https://www.linkedin.com/in/sowjanya-c-v"
            target="_blank"
            rel="noopener"
            >Sowjanya</a
          >
        </p>
        <p class="mb-0 small">© 2025, Sowjanya Chandra Vijaya</p>
      </div>
    </footer>
  </main>
</template>

<style scoped>
.main-container {
  font-family: "Domine", serif;
}

.site-footer {
  background-color: #210106;
}
.site-footer .footer-link {
  color: #fff;
  text-decoration: underline;
}
.site-footer .footer-link:hover {
  color: #f8f9fa;
  text-decoration: none;
}
</style>
