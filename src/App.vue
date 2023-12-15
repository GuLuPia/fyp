<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <div>
    <Components-Panel>
    </Components-Panel>
  </div>
  
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

import ComponentsPanel from './components/ComponentsPanel.vue';
// import HighlightTechniques from './components/HighlightTechniques.vue'

export default {
  components: {
    'Components-Panel': ComponentsPanel,
    // 'Highlight-Techniques': HighlightTechniques
  }
  // 其他组件选项和逻辑在这里
}
// export default {
//   name: 'App',
//   components: {
//     HelloWorld
//   }
// }
</script>

<style>
.Panel-Title {
  background-color: #D9D9D9;
  padding: 9px;
  display: inline-block;
  font-size: 22px;
}
.Panel-Border {
  width: 100%; 
  border: 2px solid #D9D9D9; 
}

/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
