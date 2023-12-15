<template>
    <div class="Dimension-Title">
        <div>Highlight Techniques</div>
    </div>

    <div class="Dimension-Border">
        <div>
            <div class="element">
                Light
                <div><img src="../assets/HighlightLight.svg" /></div>
            </div>

            <div class="element">
                Color
                <div><img src="../assets/HighlightColor.svg" /></div>
            </div>
        </div>
        
        <div>
            <div class="element">
                Map Pin
                <div><img src="../assets/HighlightMappin.svg" /></div>
            </div>

            <div class="element">
                3d Transformation
                <div><img src="../assets/Highlight3d.svg" /></div>
            </div>
        </div>
        
        <div>
            <div class="element">
                Map Pin
                <div><img src="../assets/HighlightEnlarge.svg" /></div>
            </div>

        </div>


        
        
        
        
        
    </div>

</template>
    
<script>

</script>
    
<style scoped>

.Dimension-Border{
    border-color: #74BBAA;
    
}

.Dimension-Title{
    background-color: #74BBAA;
    
}
.Dimension-Title {
  margin-top: 7px;
  padding: 4px;
  font-size: 18px;
  border-radius: 7px;
  display: block;
  width: 100%; 
}
.Dimension-Border {
    clear: both;
  border: 2px solid; 
  display: inline-block; 
}
.element {
    display: inline-block; /* 使 element div 成为内联块，以便整体居中 */
    text-align: center; /* 内部文本居中 */
    margin-top: 5px;
    font-size: 12px;
  }

  .element img {
    display: block; /* 使图片独占一行 */
    margin-top: 3px;
  }
</style>
    