<template>
    <div>
      <div v-if="currentSection === 'home'"> 
        <h2>Início</h2>
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
  export default {
    props: ['currentSection']
  }
  </script>
  
  <style>
  </style>
  