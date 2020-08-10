<template>
  <div>
    <Nav />
    <about/>
  </div>
</template>

<script>

import Nav from '../components/Navbar'
import about from '../components/about'

export default {
  name: 'Home',
  components: {
    Nav,
    about
  }
}
</script>
