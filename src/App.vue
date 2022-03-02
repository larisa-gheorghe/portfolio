<template>
  <Header />
  <section id="about">
    <about />
  </section>
</template>

<script>
import Header from '@/components/Header.vue';
import About from '@/components/About.vue';

export default {
  name: 'App',
  components: {
    Header,
    About,
  },
};
</script>
