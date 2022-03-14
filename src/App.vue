<template>
  <Header />
  <section id="about">
    <about />
  </section>
  <section id="portfolio">
    <portfolio />
  </section>
</template>

<script>
import Header from '@/components/Header.vue';
import About from '@/components/About.vue';
import Portfolio from '@/components/Portfolio.vue';

export default {
  name: 'App',
  components: {
    Header,
    About,
    Portfolio,
  },
};
</script>
