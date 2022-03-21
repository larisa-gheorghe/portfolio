<template>
  <Header />
  <section id="about" class="dark-sections">
    <about />
  </section>
  <section id="portfolio" class="light-sections">
    <portfolio />
  </section>
  <section id="skills">
    <skills />
  </section>
  <section id="experience" class="light-sections">
    <experience />
  </section>
  <section id="end">
    <end-section />
  </section>
</template>

<script>
import Header from '@/components/Header.vue';
import About from '@/components/About.vue';
import Portfolio from '@/components/Portfolio.vue';
import Skills from '@/components/Skills.vue';
import Experience from '@/components/Experience.vue';
import EndSection from '@/components/EndSection.vue';

export default {
  name: 'App',
  components: {
    Header,
    About,
    Portfolio,
    Skills,
    Experience,
    EndSection,
  },
};
</script>
