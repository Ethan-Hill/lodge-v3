<template>
  <div>
    <h1 v-if="error.statusCode === 404">Page not found</h1>
    <h1 v-else>An error occurred</h1>
    <NuxtLink to="/">Home page</NuxtLink>
  </div>
</template>

<style scoped>

@import url(https://fonts.googleapis.com/css?family=Ubuntu+Mono:regular,italic,700,700italic);

body {
    display: flex;
    justify-content: center;
    align-items: center;
}
div {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    max-width: 100vw;
    min-height: 90vh;
    font-family: 'Ubuntu Mono';
  }
</style>
  

<script>
  export default {
    props: ['error'],
    layout: 'error' // you can set a custom layout for the error page
  }
</script>