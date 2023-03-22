<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="">
    <small>
      <h1>Hola mundo</h1>
    </small>
    
    <hr >
    <h2>Contador: {{ contador }}</h2>
    <button @click="incrementar()">+1</button>
    <button @click="disminuir()">-1</button>
    <button @click="resetear()">Reset</button>
  </div>
</template>
<script>
  export default{
    data: () => ({
      contador:10,
    }),
    methods: {
      incrementar(){
        this.contador++;
      },
      disminuir(){
        this.contador--;
      },
      resetear(){
        this.contador = 10;
      },
    },
  }
</script>
<style scoped>
.container{
  text-align: center;
}
h1{
 color: blue;
}
h1{
  font-size: 2.5rem;
}
small{
  color: 666;
}
button{
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 6px
}
</style>