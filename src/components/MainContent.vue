<template>
  <div class="main-content">
    <div v-if="currentSection === 'home'" class = "section"> 
      <MyHome/>
    </div>
    <div v-else-if="currentSection === 'about'" class = "section">
      <MyAbout/>
    </div>
    <div v-else-if="currentSection === 'qualifications'" class = "section"> 
      <h2>Qualificações</h2>
    </div>
    <div v-else-if="currentSection === 'hobbies'" class = "section"> 
      <h2>Hobbies</h2>
    </div>
  </div>
</template>
  
<script>
  import MyHome from './MyHome.vue';
  import MyAbout from './MyAbout.vue';
  export default {
    props: ['currentSection'],
    components: {MyHome, MyAbout}
  }
</script>
  
<style scoped>
.main-content {
  padding: 20px;
  background-color: #f8f8f8;
  min-height: calc(100vh - 120px);
}
.section {
  margin: 40px 0;
  padding: 20px;
  background-color: #fff;
  box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1);
  border-radius: 5px;
}
</style>
  