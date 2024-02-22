<template>

  <div>
    <Components-Panel>
    </Components-Panel>
  </div>
  <!-- <div>
    <Canvas-Panel></Canvas-Panel>
  </div> -->
  
</template>

<script>


import ComponentsPanel from './components/ComponentsPanel.vue';
// import CanvasPanel from './components/CanvasPanel.vue';

export default {
  components: {
    'Components-Panel': ComponentsPanel,
    // 'Canvas-Panel': CanvasPanel
  }
  
}

</script>

<style>
.Panel-Title {
  background-color: #D9D9D9;
  padding: 9px;
  display: inline-block;
  font-size: 22px;
}
.Panel-Border {
  width: fit-content; 
  border: 2px solid #D9D9D9; 

  margin-top: 9px;
  margin-left: 9px;
}



</style>
