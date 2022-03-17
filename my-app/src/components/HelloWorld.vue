<template lang="">
<div v-for="personaje in personajes" :key='personaje.name'>
  <p>{{ personaje.name }}:</p>
</div>
</template>
<script>
import axios from "axios";
export default {
   data () {
    return {
      personajes: null
    }
  },
  mounted() {
    axios.get("https://swapi.dev/api/people")
    .then(response => (this.personajes = response.data.results))
  }
};
</script>
<style lang="">
  
</style>
