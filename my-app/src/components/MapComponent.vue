<script setup>
import InlineSvg from 'vue-inline-svg';
import { defineProps } from 'vue'
defineProps(['estados'])


const colourCountries= (elem, data) => {
  console.log(data)
  const mapa= elem
  for ( var country = 0 ; country< data.length; country++){
    colourCountry(data[country], mapa)
  }

}

const colourCountry =( data, mapa)=>{
  var country = mapa.getElementById(data)
  country.style.fill= '#DF583D';
}



 
</script>

<template>
  <main>
    
    <inline-svg :src="require('../assets/Mexico_templat.svg')"
    @loaded="colourCountries($event, estados)" ></inline-svg>

  </main>
</template>