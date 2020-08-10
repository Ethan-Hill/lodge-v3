<template>
  <section id="hero">
  <img id="logo" src="../assets/logo.png">
    <h1 id="title">International Lodge</h1>
    <h3 id="desc">A small community growing large</h3>
    <br>
    <b-button rounded ><a href="https://discord.gg/nVHHYQu">Click me</a></b-button>
  </section>
</template>

<style scoped>

#logo {
    border-radius: 50%;
}

#title {
    color: white;
    font-size: 40px;
    font-weight: bold;
}

#desc {
    color: white;
    font-size: 20px;
    font-weight: bold;
}

#hero {
  background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  min-height: 88.7vh;
  background-color: #fff;
}

@keyframes gradient {
	0% {
		background-position: 0% 50%;
	}
	50% {
		background-position: 100% 50%;
	}
	100% {
		background-position: 0% 50%;
	}
}
</style>
