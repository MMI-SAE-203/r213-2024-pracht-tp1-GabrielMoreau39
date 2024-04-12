<script setup lang="ts">
import { ref } from 'vue';

const maVar = ref(0)
</script>

<template>
  <p>Page accordéon</p>
  <p>la variable vaut : {{ maVar }}</p>
  <div>
    <button @click="maVar = maVar === 1 ? 0 : 1">Montrer 1</button>
    <h1 v-show="maVar === 1"
    class="text-2xl">Contenu de 1
    </h1>
  </div>
  <div>
    <button @click="maVar = maVar === 2 ? 0 : 2">Montrer 2</button>
    <h1 v-show="maVar === 2"
    class="text-2xl">Contenu de 2
    </h1>
  </div>
  <div>
    <button @click="maVar = maVar === 3 ? 0 : 3">Montrer 3</button>
    <h1 v-show="maVar === 3"
    class="text-2xl">Contenu de 3
    </h1>
  </div>
</template>