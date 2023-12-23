<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'

import {PetApi} from "../../generated/api";

const petApi = new PetApi()

console.log((await petApi.getPetById(10)).data.)
</script>

<template>
  <main>
    <TheWelcome />
  </main>
</template>
