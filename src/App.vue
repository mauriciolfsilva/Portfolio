<template>
  <div id="app">
    <MyNavbar @change-section="updateSection" />
    <MainContent :currentSection="currentSection" />
    <MyFooter />
  </div>
</template>

<script>
import MyNavbar from './components/MyNavbar.vue';
import MainContent from './components/MainContent.vue';
import MyFooter from './components/MyFooter.vue';

export default {
  components: {
    MyNavbar,
    MainContent,
    MyFooter
  },
  data() {
    return {
      currentSection: 'home'
    };
  },
  methods: {
    updateSection(section) {
      this.currentSection = section;
    }
  }
}
</script>

<style>
/* Estilos gerais do seu site */
</style>
