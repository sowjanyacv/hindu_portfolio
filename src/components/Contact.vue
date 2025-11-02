<template>
  <section
    id="contact"
    class="contact-section d-flex align-items-center justify-content-center text-center py-5"
  >
    <div class="contact-card p-4 p-lg-5">
      <blockquote class="contact-quote mb-4">
        “I aspire to craft strategies that don’t just build brands but build
        bridges, connecting people, cultures, and ideas through creativity and
        strategic insight.”
      </blockquote>

      <div
        class="contact-actions d-flex flex-column flex-sm-row gap-5 justify-content-center"
      >
        <a
          class="btn btn-outline-light btn-lg"
          href="https://www.linkedin.com/in/hindu-priya-chandra-vijaya-1618a3342/"
          target="_blank"
          rel="noopener"
        >
          <i class="bi bi-linkedin text-white me-2"></i>

          LinkedIn
        </a>

        <a class="btn btn-outline-light btn-lg" :href="`mailto:${email}`">
          <i class="bi bi-envelope-at-fill text-white me-2"></i>
          Mail
        </a>

        <a
          class="btn btn-outline-light btn-lg"
          href="https://hindupriyacv24.wixsite.com/the-in-between"
          target="_blank"
          rel="noopener"
        >
          <i class="bi bi-at text-white me-2"></i>
          Wix
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
const email = "hindupriyacv24@gmail.com ";
</script>

<style scoped>
#contact {
  background-color: #210106;
  padding: 10rem 6rem;
}

.contact-section {
  min-height: 60vh;
  background: transparent;
}
.contact-card {
  max-width: 880px;
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.02),
    rgba(255, 255, 255, 0.01)
  );
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 1rem;
  backdrop-filter: blur(6px);
}
.contact-quote {
  color: #fff;
  font-size: clamp(1rem, 1.6vw, 1.25rem);
  line-height: 1.6;
  margin: 0 0 1rem 0;
}
.contact-actions .btn {
  min-width: 10rem;
}
@media (min-width: 576px) {
  .contact-actions {
    flex-direction: row;
  }
}
</style>
