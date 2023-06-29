<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
export default {
  components: { AppHeader, AppMain, AppFooter },
  data() {
    return {

    }
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Open Sans', sans-serif;
}

.container {
  max-width: 970px;
  margin: auto;
}

img {
  max-width: 100%;
  height: auto;
}
</style>