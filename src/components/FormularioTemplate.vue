<template>
  <form>
    <label for="titulo">Título: </label>
    <input id="titulo" type="text" v-model="titulo">
    <br><hr>
    <label for="emoji">Emoji: </label>
    <select name="emoji" id="emoji" v-model="emoji">
      <option value="👨‍💻">👨‍💻</option>
      <option value="👩‍💻">👩‍💻</option>
      <option value="🦖">🦖</option>
      <option value="🧑‍💻">🧑‍💻</option>
      <option value="🙃">🙃</option>
      <option value="(ᓀ‸ᓂ)">(ᓀ‸ᓂ)</option>
    </select>
    <br><hr>
    <label >Apreciación: </label>
    <input type="radio" name="apreciacion" id="Regular" value="Regular" v-model="apreciacion">
    <label for="Regular">Regular</label>
    <input type="radio" name="apreciacion" id="Bien" value="Bien" v-model="apreciacion">
    <label for="Bien">Bien</label>
    <input type="radio" name="apreciacion" id="Muy bien" value="Muy bien" v-model="apreciacion">
    <label for="Muy bien">Muy bien</label>
    <input type="radio" name="apreciacion" id="Increible" value="Increible" v-model="apreciacion">
    <label for="Increible">Increible</label>
    <br><hr>
    <label >Competencias aprendidas: </label>
    <input type="checkbox" name="competencias" id="morfologia" value="Morfología de un componente" v-model="competencias">
    <label for="morfologia">Morfología de un componente</label>
    <input type="checkbox" name="competencias" id="directivas" value="Directivas" v-model="competencias">
    <label for="directivas">Directivas</label>
    <input type="checkbox" name="competencias" id="binding" value="One-Way y Two-Way data binding" v-model="competencias">
    <label for="binding">One-Way y Two-Way data binding</label>
    <input type="checkbox" name="competencias" id="estado" value="Estado" v-model="competencias">
    <label for="estado">Estado</label>
    <input type="checkbox" name="competencias" id="mvvm" value="El patrón de diseño MVVM" v-model="competencias">
    <label for="mvvm">El patrón de diseño MVVM</label>
    <br><hr>
    <label for="opinion">Opinión: </label>
    <textarea name="opinion" id="opinion" cols="30" rows="10" v-model="opinion"></textarea>
  </form>
  <article>
    <h1>{{ emoji }}</h1>
    <h2>{{ titulo }}</h2>
    <h3>Y me parece {{ apreciacion }}</h3>
    <h4>He aprendido:<br>{{ competencias.join(", ") }}</h4>
    <h5>Mi opinión hasta ahora del framework es:</h5>
    <p>{{ opinion }}</p>
  </article>
  </template>

<script>
export default {
  name: 'FormularioTemplate',
  data(){
    return {
      titulo: "",
      emoji: "",
      apreciacion: "",
      competencias: [],
      opinion: "",
    }
  }
}
</script>

<style scoped>
form{
  color: white;
  background-color: black;
  padding: 2%;
  border-radius: 10px;
}
article{
  text-align: center;
}
</style>
