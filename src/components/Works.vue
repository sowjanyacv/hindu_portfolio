!
<template>
  <section id="works" class="w-100">
    <h2 class="text-white text-center mb-5">My Works</h2>
    <div class="w-100 d-flex work-gap flex-wrap justify-content-center">
      <div v-for="work in works" :key="work.id">
        <div
          @click="openLink(work.link)"
          class="card d-flex justify-content-end align-items-center overflow-hidden"
          style="width: 13rem; height: 24rem"
        >
          <img :src="work.photo" alt="" class="about-img" />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import works from "../../public/assets/jsons/works.json";

function openLink(url) {
  window.open(url, "_blank");
}
</script>

<style scoped>
#works {
  padding: 10rem 6rem;
}

.card {
  border: 5px solid white;
  border-radius: 4rem;
  cursor: pointer;
}

.about-img {
  height: 100%;
  object-fit: contain;
  object-position: bottom center;
  display: block;
}

.work-gap {
  gap: 7rem;
}
</style>
