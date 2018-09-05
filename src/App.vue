<template>
  <div id="app">
    <img  id="NBAlogo" alt="NBA logo" src="./assets/NBA.png">
    <section class="east-teams">
    <img  id="teams" alt="Vue logo" src="./assets/BostonCeltics.png">
    <img  id="teams" alt="Vue logo" src="./assets/BrooklynNets.png">
    <img  id="teams" alt="Vue logo" src="./assets/NYKnicks.png">
    <img  id="teams" alt="Vue logo" src="./assets/Philadelphia76ers.png">
    <img  id="teams" alt="Vue logo" src="./assets/TorontoRaptors.png">
    <img  id="teams" alt="Vue logo" src="./assets/ChicagoBulls.png">
    <img  id="teams" alt="Vue logo" src="./assets/ClevelandCavs.png">
    <img  id="teams" alt="Vue logo" src="./assets/DetroitPistons.png">
    <img  id="teams" alt="Vue logo" src="./assets/IndianaPacers.png">
    <img  id="teams" alt="Vue logo" src="./assets/MilwaukeeBucks.png">
    <img  id="teams" alt="Vue logo" src="./assets/AtlantaHawks.png">
    <img  id="teams" alt="Vue logo" src="./assets/CharlotteHornets.png">
    <img  id="teams" alt="Vue logo" src="./assets/MiamiHeat.png">
    <img  id="teams" alt="Vue logo" src="./assets/OrlandoMagic.png">
    <img  id="teams" alt="Vue logo" src="./assets/WashingtonWizards.png">
    </section>
    <section class="west-teams">
    <img  id="teams" alt="Vue logo" src="./assets/DenverNuggets.png">
    <img  id="teams" alt="Vue logo" src="./assets/MinnesotaTwolves.png">
    <img  id="teams" alt="Vue logo" src="./assets/OklahomaThunder.png">
    <img  id="teams" alt="Vue logo" src="./assets/PortlandBlazers.png">
    <img  id="teams" alt="Vue logo" src="./assets/UtahJazz.png">
    <img  id="teams" alt="Vue logo" src="./assets/GoldenStateWarriors.png">
    <img  id="teams" alt="Vue logo" src="./assets/LAClippers.png">
    <img  id="teams" alt="Vue logo" src="./assets/LALakers.png">
    <img  id="teams" alt="Vue logo" src="./assets/PhoenixSuns.png">
    <img  id="teams" alt="Vue logo" src="./assets/SacramentoKings.png">
    <img  id="teams" alt="Vue logo" src="./assets/DallasMavs.png">
    <img  id="teams" alt="Vue logo" src="./assets/HoustonRockets.png">
    <img  id="teams" alt="Vue logo" src="./assets/MemphisGrizzlies.png">
    <img  id="teams" alt="Vue logo" src="./assets/NewOrleansPelicans.png">
    <img  id="teams" alt="Vue logo" src="./assets/SanAntonioSpurs.png">
    </section>
    <ScoreBoard />
  </div>
</template>

<script>
import ScoreBoard from './components/ScoreBoard.vue'

export default {
  name: 'app',
  components: {
    ScoreBoard
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

#NBAlogo {
  height: 8em;
}

#teams {
  height: 4em;
  margin: 5px;
}


</style>
