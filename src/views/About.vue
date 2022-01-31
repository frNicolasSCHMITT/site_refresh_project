<template>
  <Navbar />
  <AboutBody />
  <Footer />
</template>

<script>

import Navbar from '@/components/Navbar.vue'
import AboutBody from '@/components/AboutBody.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'About',
  components: {
    Navbar,
    AboutBody,
    Footer,
  }
}
</script>

<style scoped>


</style>