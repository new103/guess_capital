<template>
  <div>
    <app-header></app-header>
    <app-body></app-body>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Body from "./components/Body.vue";
import Footer from "./components/Footer.vue";

export default {
  components: {
    "app-header": Header,
    "app-body": Body,
    "app-footer": Footer,
  },
  data() {
    return {};
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* html,
body {
  height: 100%;
} */

div {
  display: grid;
  grid-template-rows: auto 1fr auto;
  min-height: 100vh;
  background: #f3f3f3;
}
</style>