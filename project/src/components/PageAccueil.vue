<template>


  <div class="book-Accueil">

    <div class="top-line"></div>

    <h1 class="title">Apprendre<br>
      VueJS</h1>

    <div class="author">

      <div class="line"></div>
      <h2>StudyCorporation</h2>
      <div class="line"></div>

    </div>

  </div>


</template>

<script>
  export default {
    data() {
      return {
        message: "",
        size: "",
        color: "",
        font: ""
      }
    }
  }
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Calligraffitti&display=swap');

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    background-color: #2c3e50;
    height: 100vh;
    display: grid;
    place-items: center;

    .book-Accueil {
      width: 30%;
      height: 80%;
      background-color: white;
      background-image: url("../upload/bg.png");
      background-repeat: no-repeat;
      background-size: cover;
      margin: 30px;
    }

    .top-line {
      width: 100%;
      border: 1px solid black;
      margin-top: 50px;
    }

    .title {
      margin: 100px 0 0 26%;
      color: white;
      font-family: 'Calligraffitti', cursive;
      font-size: 40px;
      letter-spacing: 4px;
    }

    .author {
      display: flex;
      flex-direction: row;
      align-items: center;
      margin-top: 65%;

      .line {
        width: 100%;
        border: 1px solid black;
      }

      h2{
        padding: 1%;
        border: solid 2px black;
      }
    }
  }
</style>