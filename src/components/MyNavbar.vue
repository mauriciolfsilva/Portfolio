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

<style scoped>
nav {
  background: linear-gradient(45deg, #333333, #222222);
  color: white;
  padding: 10px 0;
  border-radius: 5px;
  box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.2);
}
ul {
  list-style: none;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}
li {
  margin: 0 15px;
  cursor: pointer;
  transition: transform 0.3s ease;
}
li:hover {
  transform: translateY(-3px);
}
</style>
