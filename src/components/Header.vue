<template>
  <div>
    <header>
      <div>
        <a id="github-logo" href="https://github.com/larisa-gheorghe/portfolio">
          <svg width="90" height="90" viewBox="0 0 250 250"
            style="fill:#151513;color:#fff;position:absolute;top:0;border:0;
            left:0;transform:scale(-1,1);z-index:9999"
            aria-hidden="true"><path d="M0,0 L115,115 L130,115 L142,142 L250,250 L250,0 Z"></path>
            <path d="M128.3,109.0 C113.8,99.7 119.0,89.6 119.0,89.6 C122.0,82.7 120.5,78.6
            120.5,78.6 C119.2,72.0 123.4,76.3 123.4,76.3 C127.3,80.9 125.5,87.3 125.5,87.3
            C122.9,97.6 130.6,101.9 134.4,103.2" fill="white" style="transform-origin:130px 106px"
            class="octo-arm"></path><path d="M115.0,115.0 C114.9,115.1 118.7,116.5 119.8,115.4
            L133.7,101.6 C136.9,99.2 139.9,98.4 142.2,98.6 C133.8,88.0 127.5,74.4 143.8,58.0
            C148.5,53.4 154.0,51.2 159.7,51.0 C160.3,49.4 163.2,43.6 171.4,40.1 C171.4,40.1
            176.1,42.5 178.8,56.2 C183.1,58.6 187.2,61.8 190.9,65.4 C194.5,69.0 197.7,73.2
            200.1,77.6 C213.8,80.2 216.3,84.9 216.3,84.9 C212.7,93.1 206.9,96.0 205.4,96.6
            C205.1,102.4 203.0,107.8 198.3,112.5 C181.9,128.9 168.3,122.5 157.7,114.1 C157.9,116.9
            156.7,120.9 152.7,124.9 L141.0,136.5 C139.8,137.7 141.6,141.9 141.8,141.8 Z"
            fill="white" class="octo-body"></path></svg>
        </a>
      </div>
      <div class="row d-flex align-items-center justify-content-center text-center div-max-height">
        <div class="col-md-12">
          <i id="laptop" class="fa-solid fa-laptop-code"></i>
          <br>
          <h1 class="mb-0">Larisa Zaharia</h1>
          <div>FRONT-END DEVELOPER</div>
          <br>
          <div class="switch-mode d-flex justify-content-center">
            <div class="col-4 align-items-center">
              <input type="checkbox" id="switch" name="theme" @change="darkMode">
              <div class="app mx-auto">
                <div class="switch-body d-flex">
                  <label for="switch">
                    <div class="toggle"></div>
                    <div class="names d-flex justify-content-between">
                      <p class="light"><i class="fa-solid fa-sun"></i></p>
                      <p class="dark"><i class="fa-solid fa-moon"></i></p>
                    </div>
                  </label>
                </div>
              </div>
            </div>
          </div>

        </div>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  name: 'Header',
  mounted() {
    const theme = localStorage.getItem('data-theme');
    document.body.setAttribute('data-theme', theme);
  },
  methods: {
    darkMode() {
      // const theme = document.body.getAttribute('data-theme');
      const theme = localStorage.getItem('data-theme');
      const changeThemeToDark = () => {
        document.body.setAttribute('data-theme', 'dark');
        localStorage.setItem('data-theme', 'dark');
      };

      const changeThemeToLight = () => {
        document.body.setAttribute('data-theme', 'light');
        localStorage.setItem('data-theme', 'light');
      };

      if (theme === 'dark' && document.body.getAttribute('data-theme') === null) {
        changeThemeToDark();
      } else if (theme === 'dark' && document.body.getAttribute('data-theme') !== null) {
        changeThemeToLight();
      } else {
        changeThemeToDark();
      }
    },
  },
};
</script>
