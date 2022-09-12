<script>
  export default {
    data: () => ({
      contador: 500,
    }),
    methods: {
      saludar() {
        console.log("Hola 4A");
      },
      incrementar() {
        this.contador++;
      },
      decrementar() {
        this.contador--;
      },
      resetear() {
        this.contador = 500;
      },
    },
  };
</script>

<template>
 <!-- Button trigger modal -->
<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#staticBackdrop">
  Clic para ver la información del estudiante
</button>

<!-- Modal -->
<div class="modal fade" id="staticBackdrop" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="staticBackdropLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="staticBackdropLabel">Luis Miguel Cruz Linares 4A DSM</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body">
        Aplicaciones Web orientada a servicios
        <br>
        TI: Desarrollo de Software Multiplataforma
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        
      </div>
    </div>
  </div>
</div>

    <div class = "container">
    <img src="./assets/logo.svg" alt="Logo VUE" width="125" heigh="125">
    <small>
    <h1> Hola desde VUE.JS 3 </h1>
  </small>
    <hr>
  
    <h2>Contador {{contador}}</h2>

    <button @click="incrementar()"> +1 </button>
    <button @click="decrementar()"> -1 </button>
    <button @click="resetear()"> Reset </button>
    </div>
  </template>
  
  <style scoped>
    .container {
    text-align: center;
    }
    small {
      color: #666;
    }
    h1 {
      font-weight: bolder;
    }
    h2 {
      font-size: 2.5rem;
    }
    button {
      cursor: pointer;
      font-size: 1.5rem;
      margin: 0px 8px;
    }
  </style>