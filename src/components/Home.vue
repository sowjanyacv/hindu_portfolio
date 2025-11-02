<template>
  <section
    class="vh-100 position-relative d-flex flex-column align-items-center justify-content-end"
  >
    <img
      class="home-image-height"
      src="../assets/images/Hindu-Home.png"
      alt=""
    />
    <button
      type="button"
      class="btn btn-lg btn-outline-light home-button-position mt-2"
    >
      Hindu Priya Chandra Vijaya
    </button>
  </section>
</template>

<script setup></script>

<style scoped>
.home-image-height {
  height: 90%;
}

.home-button-position {
  position: absolute;
  bottom: 6rem;
  z-index: 10;
  font-size: 24px;
  font-weight: 800;
  pointer-events: none;
}
</style>
