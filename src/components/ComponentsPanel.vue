<template>
  <div class="Panel-Border">
    <div class="Panel-Title">
      Components Panel
    </div>

    <div id="Highlight">
      <Highlight-Techniques></Highlight-Techniques>
    </div>




  </div>
</template>
  
<script>
import HighlightTechniques from './HighlightTechniques.vue'
export default {
  components: {
    'Highlight-Techniques': HighlightTechniques
  }
}
</script>
  
<style>
/* .Dimension-Title {
  margin-top: 7px;
  padding: 4px;
  font-size: 18px;
  border-radius: 7px;
 
}
.Dimension-Border {
  border: 2px solid; 
  display: inline-block; 
} */

#Highlight {
  margin-left: 15px;
}

</style>
  