<template>
  <div>
    <div v-if="currentSection === 'home'"> 
      <MyHome/>
    </div>
    <div v-else-if="currentSection === 'about'">
      <h2>Sobre</h2>
    </div>
    <div v-else-if="currentSection === 'qualifications'"> 
      <h2>Qualificações</h2>
    </div>
    <div v-else-if="currentSection === 'hobbies'"> 
      <h2>Hobbies</h2>
    </div>
  </div>
</template>
  
<script>
  import MyHome from './MyHome.vue';
  export default {
    props: ['currentSection'],
    components: {MyHome}
  }
</script>
  
<style>
</style>
  