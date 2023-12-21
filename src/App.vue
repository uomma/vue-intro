<script >
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  data() {
    return {

     
    }
  },
  components: {
    AppHeader,
      AppMain,
      AppFooter,
  }
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppMain></AppMain>
  <AppFooter></AppFooter>
</template>

<style lang="scss">
@use './styles/variables.scss' as *;
@use './styles/general.scss' as *;

h1 {
  color: $primary-color;

  span {
    color: yellow;
  }
}
</style>
