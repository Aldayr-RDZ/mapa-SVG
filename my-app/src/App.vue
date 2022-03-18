<template>
  
  <MapComponent :estados="estados"/>
</template>

<script setup>

import { ref } from 'vue'
import MapComponent from './components/MapComponent.vue'


const estados = ref([ 'MX-1','MX-19'])



</script>

<style>

</style>
