<template>
  <div class="book">
    <Page1 v-if="count === 1"></Page1>
    <Page2 v-else-if="count === 2"></Page2>
    <Page3 v-else-if="count === 3"></Page3>
    <Page4 v-else-if="count === 4"></Page4>
    <Page5 v-else-if="count === 5"></Page5>
    <Page6 v-else-if="count === 6"></Page6>
  </div>
  <input type="number" v-model="count" name="count" id="" min="1" max="6">
</template>

<script>
import PageAccueil from "./components/PageAccueil.vue"
import Page5 from './components/Page5.vue';
import Histoire from './components/Histoire.vue'
import Installation from './components/Installation.vue'
import Syntaxe from './components/Syntaxe.vue'
import Sommaire from './components/Sommaire.vue'

export default {
  name: 'App',
  components:{
    'Page1': PageAccueil,
    'Page2': Sommaire,
    'Page3': Histoire,
    'Page4': Installation,
    'Page5': Page5,
    'Page6': Syntaxe
  },
  data () {
    return {
      count: 1
    }
  },
}

</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Calligraffitti&display=swap');
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: 'Calligraffitti', cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 100vh;
  display: grid;
  place-items: center;
}

.book{
  width: 30%;
  height: 80%;
  position: relative;
  padding: 30px;
  box-shadow: 0 4px 8px rgba($color: #000000, $alpha: 0.2);
}

input{
  position: absolute;
  bottom: 20px;
}

</style>