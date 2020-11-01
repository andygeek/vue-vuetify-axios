<template>
  <div>
    <v-container>
      <v-row>
        <button @click="getPokemon">Click me</button>
      </v-row>
    </v-container>
  </div>
</template>
<script>
import axios from "axios"
export default {
  methods: {
    async getPokemon(){
      console.log(axios);
      const datos = await axios.get("https://pokeapi.co/api/v2/pokemon/ditto");
      console.log(datos);
    }
  }
}
</script>