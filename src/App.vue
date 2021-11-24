<template>
  <div id="app">
    <!-- HEADER -->
    <Header />

    <!-- MAIN -->
    <main>
      <Hero />
      <Comics />
      <Tools />
    </main>

    <!-- FOOTER -->
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Hero from '@/components/Hero.vue';
import Comics from '@/components/Comics.vue';
import Tools from '@/components/Tools.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    Comics,
    Tools,
    Footer,
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: sans-serif;
}

#app {
  cursor: default;
}

a {
  text-decoration: none;
}

ul {
  list-style: none;
}

</style>
