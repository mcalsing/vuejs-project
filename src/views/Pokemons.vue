<template>
  <div class="container" id="app">
    <div class="columns">
      <div class="column" v-for="pokemon in pokemons">
        <div class="card">
            <div class="card-image">
            <figure class="image is-3by3">
                <img v-bind:src="pokemon.image" alt="Placeholder image">
            </figure>
            </div>
            <div class="card-content">
            <div class="media">
                <div class="media-content">
                <p class="title is-4">{{pokemon.name}}</p>
                </div>
            </div>
            <div class="content">
            <p>Type: {{pokemon.type}}</p>
            <span>Weight: {{pokemon.averageWeight.value}}</span>
            <span>{{pokemon.averageWeight.measurementUnit}}</span>
                <br>
            </div>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import pokemonsData from "@/assets/data"

export default {
  name: 'pokemons',
  data() {
    return {
      pokemons: pokemonsData,
    }
  }
}
</script>

<style scoped>
.image {
  border: 1px solid gray
}

</style>

