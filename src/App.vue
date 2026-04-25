<script> 
 export default{
  data: () => ({
    contador: 10,
  }),
  methods: {
    incrementar(){
      this.contador++;
    },
    disminuir(){
      this.contador--;
    },
    reset(){
      this.contador = 0;
    }
  },
 };

</script>
<template> 
  <div class="container">

        <img src="./assets/android-vertical.svg" alt="Logo Juxe" width="125" height="125" />
        <small>
          <h1> Tacos de guayaba </h1>
        </small>
        <hr/>

        <h2>Contador: {{contador}}</h2>
        <button @click="incrementar()">+1</button>
        <button @click="disminuir()">-1</button>
        <button @click="reset()">Reset</button>
        </div>
      </template>

      <style scoped>
      

      .container {
        text-align: center;

      }
      small {
        color: blueviolet;
      }
        
      h1 {
        font-weight: bolder;
      }
      h2{
        font-size: 2rem;
      }

      button{
        cursor: pointer;
        font-size: 1.5rem;
        margin: 0px 6px;
      }
        

      </style>          