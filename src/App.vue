<script>
export default {

    data: () =>({
      contador:10,
    }),
    methods:{
      saludar(){
        console.log("hola")
      },
      incrementar(){
        this.contador++;
      },
      decrementar(){
        this.contador--;
      },
      resetear(){
        this.contador=10;
      },
    },
  };

</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="logo" width="100px" height="100px" >
    <small>
  <h1>Hola Mundo desde Vue js 3 </h1>
</small>
  <hr><br>
  <div class="contador">
    <h2>CONTADOR {{ contador }}</h2><br>
        <button @click="incrementar()">+1</button>
      <button @click="decrementar()">-1</button>
      <button @click="resetear()">Reset</button>
  </div>
  <hr/>

</div>
  </template>
  <style scoped>

  .container{
    font-family: Lato sans-serif;
    text-align: center;
  }
  small{
    color:#555;
  }
  .h1{
    color:red;
    font-weight: bolder;
  }
.contador{
  max-width: 400px;
  max-width: 300px;
}
h2{
  font-size: 2.5rem;
}
button{
  cursor:pointer;
  font-size: 1.5rem;
  margin: 0px 6px;
}
</style>