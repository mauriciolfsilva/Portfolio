<template>
  <body>
    <h2>Quem sou eu?</h2>
    <div>
      <p>{{ getIntro(getYear) }}</p>
    </div>
  </body>
</template>
  
<script>
  export default {
    methods: {
      getYear(dataStr) {
        const today = new Date();
        const data = new Date(dataStr);
        
        let age = today.getFullYear() - data.getFullYear();
        const monthActual = today.getMonth();
        const monthdata = data.getMonth();
        
        if (monthActual < monthdata || (monthActual === monthdata && today.getDate() < data.getDate())) {
          age--;
        }
        return age;
      },
      getIntro(yearF) {
        return "Olá, sou Mauricio, um entusiasta da tecnologia e amante da programação, com " +
               `${yearF('1998-12-18')} anos de idade e ${yearF('2014-01-01')} anos de imersão apaixonada nesse universo fascinante. ` +
               "Desde o momento em que mergulhei no mundo da codificação, descobri não apenas " +
               "uma habilidade, mas sim uma paixão avassaladora. " +
               "Como desenvolvedor e aspirante a cientista da computação, encontrei na programação " +
               "não apenas linhas de código, mas sim a oportunidade de criar soluções, moldar o futuro " +
               "e desvendar os mistérios do mundo digital. Cada desafio enfrentado é uma oportunidade para " + 
               "explorar novas possibilidades, aprimorar minhas habilidades e contribuir para um mundo " + 
               "impulsionado pela inovação tecnológica. Neste espaço, compartilho não apenas meu trabalho, " + 
               "mas também meu amor pela programação. É uma jornada contínua de aprendizado, crescimento e " + 
               "uma imensa gratificação ao ver ideias se transformarem em realidade através do poder do código. " +
               "Junte-se a mim enquanto navego por esse fascinante mundo da tecnologia, explorando novas fronteiras " + 
               "e expandindo os horizontes da computação."
      }
    }
  }
</script>
  
<style>
</style>
  