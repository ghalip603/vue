<template>
  <div id="nav">

    <div class="ToHomeLogo">
      <img src="../src/assets/logo.png" alt="Logo">
      <a href="src/views/Home.vue">Www.Tanxianit.Com</a>
    </div>
    <router-link to="/">Home</router-link>
    <router-link to="/blog">Blog</router-link>
    <router-link to="/tutorials">Tutorials</router-link>
    <router-link to="/about">About</router-link>
  </div>
  <router-view />
</template>
<script>
export default {
  name: "app"

}
;
</script>
<style lang="scss">
#app {
  font-family: 'Lato', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}


body {
  margin: 0;
  padding: 0;
}

#nav {
  display: flex;
  justify-content: flex-end;
  width: 100%;
  height: 60px;
  background: #2c3e50;
  align-items: center;

  a {
    font-weight: bold;
    color: #efebeb;
    text-decoration: none;
    margin: 8px;
    padding: 12px;
    border: 2px;

    &.router-link-exact-active {
      color: #42b983;
    }
  }

  .ToHomeLogo {
    width: 70%;
    display: flex;
  }

  .ToHomeLogo img {
    width: 40px;
    height: 40px;
    padding: 2px;
    margin: 8px;
  }
}

</style>
