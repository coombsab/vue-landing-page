<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <main>
    <router-view />
  </main>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  flex-direction: column;
  height: 100vh;
  background-color: rgba(0, 0, 0, 0.9);
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

main {
  display: flex;
  flex-direction: column;
  flex-grow: 1;
}

body {
  width: 100vw;
  height: 100vh;
  background-color: black;
  background-image: url("https://i.giphy.com/media/OK5LK5zLFfdm/giphy.webp");
  background-position: center;
  background-size: cover;
  display: flex;
  flex-direction: column;
  margin: 0;
}

.body-wrapper {
  background-color: rgba(0, 0, 0, 0.9);
  height: 100%;
  width: 100%;
}

.text-visible {
  text-shadow: 2px 0 2px rgba(0, 0, 0, 0.644), 0 2px 2px rgba(0, 0, 0, 0.644), -2px 0 2px rgba(0, 0, 0, 0.644), 0 -2px 2px rgba(0, 0, 0, 0.644), 0 0 10px rgba(255, 4, 4, 0.846);
  color: rgb(241, 231, 231);
  font-weight: 700;
  letter-spacing: 0.035rem;
}
</style>
