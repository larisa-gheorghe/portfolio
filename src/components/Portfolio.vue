<template>
  <div class="col-md-12">
    <h1 class="text-center pt-5 pb-4 section-title">
        <span>Projects</span>
    </h1>
    <div class="col-md-12 mx-auto">
      <div class="row mx-auto">
          <div class="col-sm-12 col-md-6">
            <span class="portfolio-item text-center d-block mb-4">
              <div class="foto" @click="redirectToWeddingApp">
                  <div>
                    <img src="../../public/assets/img/wedding.jpg" alt="" class="mb-0 pb-0 d-block">
                    <span class="project-date">2022</span>
                    <br>
                    <p class="mt-3">Wedding Invitation</p>
                  </div>
              </div>
            </span>
          </div>
          <div class="col-sm-12 col-md-6">
            <span class="portfolio-item text-center d-block mb-4">
              <div class="foto" @click="redirectToMusicApp">
                  <div>
                    <img src="../../public/assets/img/music.jpg" alt="" class="mb-0 pb-0 d-block">
                    <span class="project-date">2021</span>
                    <br>
                    <p class="mt-3">Music App</p>
                  </div>
              </div>
            </span>
          </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Portfolio',
  methods: {
    redirectToWeddingApp() {
      window.location.href = 'https://vue-wedding-app.pages.dev/';
    },
    redirectToMusicApp() {
      window.location.href = 'https://vue-music-app.pages.dev/';
    },
  },
};
</script>
