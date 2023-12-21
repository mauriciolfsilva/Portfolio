<template>
    <nav>
      <ul>
        <li @click="changeSection('home')">Início</li>
        <li @click="changeSection('about')">Sobre</li>
        <li @click="changeSection('qualifications')">Qualificações</li>
        <li @click="changeSection('hobbies')">Hobbies</li>
      </ul>
    </nav>
  </template>
  
  <script>
  export default {
    methods: {
      changeSection(section) {
        this.$emit('change-section', section);
      }
    }
  }
  </script>
  
  <style>
  </style>
  