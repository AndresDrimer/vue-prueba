
<template>
<TheHeader />
  <h1> Esto ya esta en el main de App</h1>
  <h2 :name="name">Inserto un nombre : {{ name }} y ademas le paso un valor: {{ number }}</h2>
  <input type="text" v-model="name">
  <button :click="number++">sumar uno</button>


<TheFooter />
</template>

<script setup>
import TheHeader from './components/TheHeader.vue';
import { ref } from 'vue';
import TheFooter from './components/TheFooter.vue';
components: { TheHeader, TheFooter };
let name = ref("");
let number = ref (0)


</script>


<style scoped>

</style>
