<template>
  <div>
    <h1>{{ this.count }}</h1>
    <button @click="increment">+</button>
  </div>
</template>

<script>
import { mapState } from 'vuex'

export default {
  computed: mapState([
    'count'
  ]),
  methods: {
    increment () {
      this.$store.commit('increment')
    }
  },
};
</script>

<style>
.done {
  text-decoration: line-through;
}
</style>
