<template>
  <div id="app">
    <TheHeader/>
    <TheMain/>
    <TheFooter/>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheMain from './components/TheMain.vue';
import TheFooter from './components/TheFooter.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheMain,
    TheFooter
}
}
</script>

<style lang="scss">
@import "./assets/scss/main.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}

.container {
    max-width: 1000px;
}

a {
    color: black;
    text-decoration: none;
}
</style>
