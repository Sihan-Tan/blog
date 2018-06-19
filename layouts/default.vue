<template>
  <div>
    <Header></Header>
    <nuxt/>
    <Footer></Footer>
    <a href="#" class="cd-top">Top</a>
  </div>
</template>

<script>
import Header from '~/components/Header.vue'
import Home from '~/components/Home.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Header,
    Home,
    Footer
  }
}
</script>

<style>
</style>
