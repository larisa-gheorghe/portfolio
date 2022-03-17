<template>
  <Header />
  <section id="about">
    <about />
  </section>
  <section id="portfolio">
    <portfolio />
  </section>
  <section id="skills">
    <skills />
  </section>
</template>

<script>
import Header from '@/components/Header.vue';
import About from '@/components/About.vue';
import Portfolio from '@/components/Portfolio.vue';
import Skills from '@/components/Skills.vue';

export default {
  name: 'App',
  components: {
    Header,
    About,
    Portfolio,
    Skills,
  },
};
</script>
