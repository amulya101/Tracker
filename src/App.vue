<script >

import Nav from './components/nav.vue'
import Header from './components/header.vue'
import Inputs from './components/inputs.vue'
import Display from './components/display.vue'

  export default {
    name: 'App',
    components: {
      Nav,
      Header,
      Inputs,
      Display
    },
    data() {
      return {
        players: [],
        //playersFormatted: []
      }      
    },
    created() { 
      this.players = [
        {
          id: 1,
          firstName: "Kepa",
          lastName: "Arrizabalaga",
          country: "Esp",
          Position: "GK"
        },
        {
          id: 2,
          firstName: "Antonio",
          lastName: "Rudiger",
          country: "GER",
          Position: "CB"
        },
        {
          id: 3,
          firstName: "Marcos",
          lastName: "ALONSO",
          country: "EsP",
          Position: "CB"
        },
        {
          id: 4,
          firstName: "Andreas",
          lastName: "Chris",
          country: "DEN",
          Position: "CB"
        },
        {
          id: 5,
          firstName: "Jorginho",
          lastName: "Frello",
          country: "ITA",
          Position: "CM"
        },
        {
          id: 6,
          firstName: "tHIAGO",
          lastName: "sILVA",
          country: "Bra",
          Position: "CB"
        },
        {
          id: 7,
          firstName: "Ngolo",
          lastName: "Kante",
          country: "Fra",
          Position: "CM"
        },
        {
          id: 8,
          firstName: "Matteo",
          lastName: "Kovacic",
          country: "Cro",
          Position: "cm"
        },
        {
          id: 9,
          firstName: "rOMELU",
          lastName: "Lukaku",
          country: "Bel",
          Position: "St"
        },
        {
          id: 10,
          firstName: "Christian",
          lastName: "pulisic",
          country: "USA",
          Position: "LW"
        },
        {
          id: 11,
          firstName: "Timo",
          lastName: "Werner",
          country: "Ger",
          Position: "ST"
        },
        {
          id: 16,
          firstName: "Edouard",
          lastName: "Mendy",
          country: "Sen",
          Position: "GK"
        },
        {
          id: 19,
          firstName: "Mason",
          lastName: "MOUNT",
          country: "enG",
          Position: "RM"
        },
        {
          id: 24,
          firstName: "Reece",
          lastName: "james",
          country: "eng",
          Position: "rb"
        },
        {
          id: 29,
          firstName: "King Kai",
          lastName: "Havertz",
          country: "GER",
          Position: "CF"
        }
      ]
      console.log(this.players[0]);

      for (let i = 0; i < this.players.length; i++) {
        this.players[i].firstName = this.players[i].firstName.toUpperCase();
        
      } 
    }

  }
</script>

<template>
  <Nav first="Home" second="About" />                  <!-- use of props -->
  <div class="container">
    <Header  />    
  </div>
  <Inputs intro="We will be here soon !!" />
  <Display teamName = "Chelsea FC" :players="players" />
</template>

<style>

.container{
  border: 3px solid blue;
  display: flex;
  width: 100%;
  font-size: 24px;
  justify-content: center;
  font-family: 'Courier New', Courier, monospace;
}

</style>
