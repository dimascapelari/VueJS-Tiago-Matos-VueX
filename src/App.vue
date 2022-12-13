<template>
  <img alt="Vue logo" src="./assets/logo.png" /><br />

  Nome: {{ $store.state.user.first_name }}<br />
  Sobrenome: {{ $store.state.user.last_name }}<br />
  E-mail: {{ $store.state.user.email }}

  <HelloWorld msg="Welcome to Your Vue.js App" />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
  data() {
    return {};
  },
  created() {
    console.log("App", this.$store);
    console.log("App", this.$store.state.user);
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
