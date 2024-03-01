<script>
import AppNavbar from './components/AppNavbar.vue'
import AppContent from './components/AppContent.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  components: {
    AppNavbar,
    AppContent,
    AppFooter
  }
}

</script>

<template>
  <AppNavbar></AppNavbar>
  <AppContent></AppContent>
  <AppFooter></AppFooter>
</template>

<style>

body{
  margin: 0;
}

</style>