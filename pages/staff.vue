<template>
  <div>
    <Nav />
    <Staff />
  </div>
</template>

<script>

import Nav from '../components/Navbar'
import Staff from '../components/staff'

export default {
  name: 'Home',
  components: {
    Nav,
    Staff
  }
}
</script>
