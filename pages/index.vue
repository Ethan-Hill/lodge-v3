<template>
  <div>
    <Nav />
    <Hero />
  </div>
</template>

<script>

import Nav from '../components/Navbar'
import Hero from '../components/Hero'

export default {
  name: 'Home',
  components: {
    Nav,
    Hero
  }
}
</script>
