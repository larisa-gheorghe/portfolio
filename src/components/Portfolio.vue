<template>
  <div class="col-md-12">
    <h1 class="text-black text-center pt-5 pb-4 section-title">
        <span>Projects</span>
    </h1>
    <div class="col-md-12 mx-auto">
      <div class="row mx-auto">
          <div class="col-sm-12 col-md-6 col-lg-4">
            <span class="portfolio-item text-center d-block mb-4">
              <div class="foto" @mouseover="zoomInProject" @click="redirect">
                  <div>
                    <img src="../../public/assets/img/wedding.jpg" alt="" class="mb-0 pb-0 d-block">
                    <span class="project-date">2020</span>
                    <br>
                    <p class="mt-3">Wedding Invitation</p>
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
    zoomInProject() {
      // const foto = document.getElementsByClassName('foto')[0];
      // foto.classList.add('zoom');
    },
    redirect() {

    },
  },
};
</script>
