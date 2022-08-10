<template>
<div>
  <h1>Hello World</h1>
</div>
<div>
  <h1>Aquí sumamos {{10 + 2}}</h1>
</div>
<div>
  <h1>String con un giro {{nombre()}}</h1>
</div>
<div>
  <h1 v-if="myAge < 30">Still on ur twenty's</h1>
</div>
<div v-for="manuals in books" v-bind:key="manuals">
  <h2 v-for="freaks in manuals" v-bind:key="freaks">{{freaks}}</h2>
</div>
</template>

<script>
export default {
  data() {
    return {
name: 'FranCesc',
myAge: '29',
books:[
  {título:"Tashas coulderon of everything", descripción: "Monstruario", contenido: "lista de monstruos en tasha"},
  {título: "Icewinday", descripción: "Ice Adventure", contenido: "20 min adventure in and out"},
  {título: "d&d", descripción: "Master Manual", contenido: "Reglas y normas"},
],

    };
  },
  methods: {
nombre(){
  
  return this.name.split("").reverse().join("");
}
  
    },
  }

</script>

<style>

</style>
