<template lang="">
<div>
<InlineSvg :src="require('../assets/Mexico_template.svg')"  type="image/svg+xml" onmouseover="displayName('Nuevo León')">
</InlineSvg>

<text class="label" id="country-name" x="10" y="390"> </text>


</div>

</template>
<script >
import InlineSvg from 'vue-inline-svg';
export default {
    components:{
        InlineSvg,
    },
     data() {
    
  },
    methods: {
       
      displayName: function (name){
          document.getElementById('').firstChild.data = name;
        }
    },
}




</script>
<style lang="">

  
</style>

