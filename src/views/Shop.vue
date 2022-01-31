<template>
  <Navbar />
  <ShopBody />
  <Footer />
</template>

<script>

import Navbar from '@/components/Navbar.vue'
import ShopBody from '@/components/ShopBody.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'Shop',
  components: {
    Navbar,
    ShopBody,
    Footer,
  }
}
</script>

<style scoped>


</style>