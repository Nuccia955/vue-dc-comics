<template>
  <div id="app">
    <!-- HEADER -->
    <Header />

    <!-- MAIN -->
    <main>
      <Contents />
      <Tools />
    </main>

    <!-- FOOTER -->
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Contents from '@/components/Contents.vue'
import Footer from '@/components/Footer.vue'
import Tools from '@/components/Tools.vue'

export default {
  name: 'App',
  components: {
    Header,
    Contents,
    Footer,
    Tools,
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
