<template>
  <section
    id="about"
    class="d-flex justify-content-center align-items-center gap-5 flex-column flex-lg-row"
  >
    <div>
      <h2 class="text-white text-center mb-4">About Me</h2>
      <p class="text-white text-center">
        I’m Hindu Priya Chandra Vijaya. I believe the best ideas live where
        insight meets imagination. I’m currently pursuing my MSc in Marketing &
        Strategy at the University of Warwick.
      </p>
      <p class="text-white text-center">
        My background in Marketing and Finance, combined with hands-on
        experience across industries such as ed-tech, skincare, sports, and
        healthcare, has taught me how to balance data with empathy, logic with
        creativity, and vision with execution.
      </p>
      <p class="text-white text-center">
        Outside of work, I’m passionate about creative writing, dance, fashion,
        and music. I also enjoy exploring new perspectives through travel and
        learning about the ways people express identity and emotion across
        cultures.
      </p>
    </div>
    <div
      class="card-border-wrapper d-flex justify-content-center align-items-center bg-light"
    >
      <div
        class="card bg-light d-flex justify-content-end align-items-center overflow-hidden"
        style="width: 18rem; height: 24rem"
      >
        <img
          src="../../public/assets/images/Hindu-About.png"
          alt=""
          class="about-img"
        />
      </div>
    </div>
    <div>
      <h2 class="text-white text-center mb-4">My Goals</h2>
      <p class="text-white text-center">
        My goal is to join an organization where I can use my strategic and
        creative skills to solve real-world challenges and drive meaningful
        change.
      </p>
      <p class="text-white text-center">
        I aspire to help shape brands and build connections with diverse
        audiences, leading teams to deliver innovative solutions that create
        lasting impact.
      </p>
      <p class="text-white text-center">
        For me, marketing is about storytelling, building connections, and
        inspiring change. I approach challenges with curiosity and strategy, and
        thrive in collaborative environments. If you value fresh ideas and a
        global perspective, let’s connect.
      </p>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
#about {
  background-color: #210106;
  padding: 10rem 6rem;
}

.card-border-wrapper {
  padding: 2px;
  border-radius: 5rem;
}

.card {
  border: 10px solid #210106;
  border-radius: 5rem;
}

.about-img {
  height: 100%;
  object-fit: contain;
  object-position: bottom center;
  display: block;
}
</style>
