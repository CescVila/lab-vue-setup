<template>
  <div>
    <h1>
      Hola mi nombre es{{ name }}, soy de {{ place }} y tengo {{ years }} años
    </h1>
  </div>
  <!-- <template v-if="display">
    <h1>Puedes tomar alcohol</h1>
    <template v-if="display" >
        <h1>No puedes tomar</h1>
        <template>
            <h1>Estás muy viejo para tomar</h1>
        </template>
    </template>

  </template> -->
</template>

<script>
export default {
  setup() {
    return{

    name: "Cesc"
    place: "BCN"
    years: "29"

  },
  }

};
</script>

<style>
.color-blue {
  background-color: blue;
}
.h1{
    font-size: 18px;
}
</style>