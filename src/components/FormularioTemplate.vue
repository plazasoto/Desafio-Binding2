<template>
  <form>
    <label for="titulo">Título: </label>
    <input id="titulo" type="text">
    <br><hr>
    <label for="emoji">Emoji: </label>
    <select name="emoji" id="emoji">
      <option value="(ᓀ‸ᓂ)">(ᓀ‸ᓂ)</option>
      <option value="ᓀ‸ᓂ">ᓀ‸ᓂ</option>
    </select>
    <br><hr>
    <label >Apreciación: </label>
    <input type="radio" name="apreciacion" id="Regular" value="Regular">
    <label for="Regular">Regular</label>
    <input type="radio" name="apreciacion" id="Bien" value="Bien">
    <label for="Bien">Bien</label>
    <input type="radio" name="apreciacion" id="Muy bien" value="Muy bien">
    <label for="Muy bien">Muy bien</label>
    <input type="radio" name="apreciacion" id="Increible" value="Increible">
    <label for="Increible">Increible</label>
    <br><hr>
    <label >Competencias aprendidas: </label>
    <input type="checkbox" name="competencias" id="morfologia" value="Morfología de un componente">
    <label for="morfologia">Morfología de un componente</label>
    <input type="checkbox" name="competencias" id="directivas" value="Directivas">
    <label for="directivas">Directivas</label>
    <input type="checkbox" name="competencias" id="binding" value="One-Way y Two-Way data binding">
    <label for="binding">One-Way y Two-Way data binding</label>
    <input type="checkbox" name="competencias" id="estado" value="Estado">
    <label for="estado">Estado</label>
    <input type="checkbox" name="competencias" id="mvvm" value="El patrón de diseño MVVM">
    <label for="mvvm">El patrón de diseño MVVM</label>
    <br><hr>
    <label for="opinion">Opinión: </label>
    <textarea name="opinion" id="opinion" cols="30" rows="10"></textarea>
  </form>
  </template>

<script>
export default {
  name: 'FormularioTemplate',
}
</script>

<style scoped>
form{
  color: white;
  background-color: black;
  padding: 2%;
  border-radius: 10px;
}
</style>
