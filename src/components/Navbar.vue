<template>
  <div id="nav">
    <router-link id="logo-url" to="/">
      <img id="logo" :src="logo" :alt="alt" />
    </router-link>
    <router-link to="/">Home </router-link>
    <router-link to="/Pedidos">Pedidos</router-link>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  props: ["logo", "alt"],
};
</script>

<style scoped>
#nav {
  background-color: #222;
  border-bottom: 4px solid #111;
  padding: 15px 50px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}
#nav #logo-url {
  margin: auto;
  margin-left: 0;
}

#logo {
  width: 40px;
  height: 40px;
}

#nav a {
  color: #fcba03;
  /* tirar o sublinhado dos links  */
  text-decoration: none;
  transition: 0.5s;
  margin: 12px;
}

#nav a:hover {
  /* ponteiro do mouse passa e fica branco  */
  color: #fff;
}
</style>