<template>
  <aside>
    <h3>Je suis ton pere</h3>
    <h5>{{ nombre }}</h5>
    <button @click="this.ajouter">plus</button>
    <!-- @ ou v-on:  les 2 ca marche / OU @click="nombre++ (sans methods:{})"-->
    <button v-on:click="this.diminuer">moins</button>

    <!-- v-model c pour relier les champs et les données -->
    <input type="number" v-model="nombre" />
  </aside>
</template>

<script>
export default {
  data() {
    return {
      nombre: 0,
    };
  },
  methods: {
    ajouter() {
      this.nombre++;
    },
    diminuer() {
      this.nombre--;
    },
  },
};
</script>

<style>
</style>