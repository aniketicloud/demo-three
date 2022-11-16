<template>
  <div id="app">
    <h1>{{ title }}</h1>
    <Input number="1" />
    <Input number="2" />

    <!-- <v-btn elevation="2"></v-btn> -->

    <div>
      {{ textOnScreen }}
    </div>
  </div>
</template>

<script>
import Input from "./components/Input.vue";

export default {
  name: "AppComponent",
  data() {
    return {
      title: "Ciao Mondo",
    };
  },
  components: {
    Input,
  },
  computed: {
    textOnScreen() {
      return "hello";
    },
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
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

h1 {
  color: red;
}
</style>

// vue directives