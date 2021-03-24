<template>
  <div id="app">
     <h1>Calculadora</h1>
     <Calculator />
  </div>
</template>

<script>
import Calculator from "./main/Calculator"


export default {
  name: 'App',
  components: {
    Calculator

  }
}
</script>

<style>
  @font-face{
    font-family: "RobotoMono";
    src: url("./fonts/RobotoMono.ttf");
  }
  *{
    font-family: "RobotoMono", monospace;
    margin:0;
    padding: 0;
    box-sizing: border-box;
  }

  h1{
    padding: 20px 0;
    font-weight: lighter;
  }

  #app{
    display: flex;
    flex-direction: column;
    height: 100vh;
    justify-content: center;
    align-items: center;
    text-align: center;
    color:#fff;
    background: linear-gradient(to right, #30042b,#000000);
  }
  @media (max-width: 500px) {
  .calculator {
    padding: 2px 15px;
    width: 100%;
  }
}
</style>
