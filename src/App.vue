<script>
  export default {
    data: () => ({
      contador : 10,
    }),
    methods: {
      saludar(){
        console.log("Hola 10A | @")
      },
      incrementar(){
        this.contador++;
      },
      decrementar(){
        this.contador--;
      },
      resetear(){
        this.contador=500;
      },
    }
  };

</script>

<template>
  <div class="alert alert-info" role="alert">
    Iztayetzy Kim Neri Gálvez 10° "A"
  </div>
  <br>
  <img src="./assets/logo.svg" alt="Logo VUE" with="125" height="125">
  <h1>Hola desde VUE.js 3</h1>
  <hr>
  <h2>Contador {{contador}}</h2>
  <button v-on:click="incrementar()">+1</button>
  <button v-on:click="decrementar()">-1</button>
  <button v-on:click="resetear()">Reset</button>
</template> 

<style scoped>
  .container{
  text-align: centers;
  }
  small{
    color: #666;
  }
  h1 {
    font-weight: bolder;
  }
  h2{
    font-size: 2.5rem;
  }
  button {
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 8px;
  }
</style>


