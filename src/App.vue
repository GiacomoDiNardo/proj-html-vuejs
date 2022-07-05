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
@import "./assets/scss/variables";
@import url('https://fonts.googleapis.com/css2?family=ABeeZee&display=swap');

#app {
  font-family: 'ABeeZee', sans-serif;
}

.container {
    max-width: 1000px;
}

a {
    color: black;
    text-decoration: none;
}

.text-grey {
  color: $text-grey;
}

.text-primary {
  color: $primary;
}

.border-grey {
  border-color: $border-grey;
}
</style>
