<template>
  <div class="container">
    <img class="background-image" alt="App logo" src="./../assets/undraw_fitness_stats_orange.png">
    <h2 class="title">{{ title }}</h2>
    <h3 class="description">{{ description }}</h3>
    <div class="wrapper">
      <div>
        <input type="text" placeholder="Peso (kg)" class="input">
      </div>
      <div>
        <input type="text" placeholder="Altura (cm)" class="input">
      </div>  
      <button type="button" class="button button-text">Calcular</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IMC',
  props: {
    title: String,
    description: String
  }
}
</script>

<!-- "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .container {
    display: flex;           /* establish flex container */
    flex-direction: column;  /* make main axis vertical */
    justify-content: center; /* center items vertically, in this case */
    align-items: center;     /* center items horizontally, in this case */
    background-color: #fbfffe;
  }
  .wrapper {
   align-self: center;
  }
  .background-image {
    height: 300px;
  }
  .head {
    align-items: center;
  }
  .title {
    font-size: 30px;
    color: #1b1b1e;
  }
  .description {
    font-size: 20px;
    color: #6d676e;
  }
  .input {
    background-color: #6d676e;
    border: none;
    border-radius: 5px;
    margin-top: 15px;
    margin-left: 0px;
    padding: 10px;
    color: #faa916;
    font-size: 20px;
  }
  .button {
    display: block;
    width: 100%;
    border: none;
    border-radius: 5px;
    margin-top: 15px;
    background-color: #faa916;
    padding: 10px;
  }
  .button-text {
    color: #fbfffe;
    font-size: 25px;
  }
</style>