<template>
  <button @click="doSomething">Click Me! {{counter}}</button>
</template>

<script setup lang="ts">
import {ref} from "vue";

const counter = ref(0)

function doSomething(){
  counter.value++;
  console.log('something happened', counter.value)
}
</script>
