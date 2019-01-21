<template>
  <div id="app">
    <div class="container">
      <h1 class="title">City Guide</h1>

      <div class="select is-primary is-rounded is-hovered ">
        <select v-model="ciutatSelected">
          <option v-for="city in llistaCiutats" :key="city">{{ city }}</option>
        </select>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        name: 'app',
        data () {
            return {
                ciutatSelected: "Barcelona",
                llistaCiutats: [
                    "Barcelona",
                    "Madrid",
                    "Berlin",
                    "Paris",
                    "Amsterdam"]
            }
        }
    }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    margin-top: 60px;
  }

  h1 {
    text-align: center;
  }
</style>
