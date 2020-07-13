<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/icon-41.png">

      <h2>Áreas de Interés</h2>        
      <MiLista title="Tecnología" v-bind:items="Tecnologia"/>
          
      <MiLista title="Ciencias Sociales" v-bind:items="Ciencias_Sociales"/>
          
      <MiLista title="Artes" v-bind:items="Artes"/>
          
      
  </div>
</template>

<script>
import MiLista from './components/MiLista.vue'

export default {
  name: 'App',
  components: {
    MiLista
  },
  data: () => {
    return {
      Tecnologia: [
        {texto:'Javascript', url:'https://www.codecademy.com/catalog/language/javascript'},
        {texto:'CSS', url:'https://www.w3schools.com/w3css/'},
        {texto:'React', url:'https://reactjs.org/tutorial/tutorial.html'},
        {texto:'Python', url:'https://www.learnpython.org/'},
        {texto:'Ruby', url:'https://www.codecademy.com/learn/learn-ruby'},
      ],
      Ciencias_Sociales: [
        {url: "https://www.ohchr.org/en/issues/pages/whatarehumanrights.aspx", texto: 'Derechos Humanos'},
        {url: "https://mcl.as.uky.edu/gender-studies", texto: 'Estudios de Género'},
        {url: "http://www.arthistory.net/", texto: 'Historia del Arte'},
        {url: "https://www.humanrightscareers.com/masters-refugees-migration/", texto: 'Trabajo con Refugiados'},
        {url: "https://www.undp.org/content/undp/en/home/ourwork/democratic-governance-and-peacebuilding/conflict-prevention-and-peacebuilding/", texto: 'Peacebuilding'}
      ],
      Artes: [
        {url: "http://www.art-class.net/06-tutorials/drawing/techniques.php", texto:'Dibujo'},
        {url: "http://www.art-class.net/06-tutorials/painting/paint-with-oil-01.php", texto:'Pintura Acrílica y en Óleo'},
        {url: "https://www.skillshare.com/browse/photography", texto:'Fotografía'},
        {url: "https://www.lahacedora.cl/taller-online-ceramica-en-frio-1", texto:'Cerámica en frío'},
        {url: "https://www.thesprucecrafts.com/what-wire-for-what-2048450", texto:'Joyería'}
      ]  
    } 
  }
}
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: goldenrod;
    margin-top: 20px;
    background-color:#1b0522;
  }

  #app img {
    max-width: 30%;
    opacity: 75%;
  }

</style>
