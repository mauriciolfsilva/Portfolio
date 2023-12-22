<template>
    <h2>Quem sou eu?</h2>
    <div>Me chamo Mauricio, tenho {{ getAge() }} anos. Sou desenvolvedor de software e futuro Cientista da Computação!</div>
    <h2></h2>
</template>
  
<script>
  export default {
    methods: {
      getAge() {
        const today = new Date();
        const birth = new Date('1998-12-18');
        
        let age = today.getFullYear() - birth.getFullYear();
        const monthActual = today.getMonth();
        const monthBirth = birth.getMonth();
        
        if (monthActual < monthBirth || (monthActual === monthBirth && today.getDate() < birth.getDate())) {
          age--;
        }
        
        return age;
      }
    }
  }
</script>
  
<style>
</style>
  