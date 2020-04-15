<template>
  <div class="nav">
    <nuxt-link to="/" class="brand">Ceoil.ie</nuxt-link>
    <nav></nav>
  </div>
</template>

<script>
export default {}
</script>

<style>
.nav {
  position: fixed;
  height: 60px;
  padding: 0 20px 0px 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 1em;
}
.nav .nav-item {
  box-sizing: border-box;
  margin: 0 5px;
  color: rgba(0, 0, 0, 0.5);
  text-decoration: none;
}
.nav .nav-item.router-link-exact-active {
  color: #39b982;
  border-bottom: solid 2px #39b982;
}
.nav a {
  display: inline-block;
}
.brand {
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
  font-size: 1.2em;
  color: #000;
  text-decoration: underline;
}
</style>