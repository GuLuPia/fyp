<template>
    <div id="map-container"></div>
  </template>
  
  <script>
  import * as d3 from 'd3';
  
  export default {
    name: 'WorldMap',
    mounted() {
      this.drawMap();
    },
    methods: {
      drawMap() {
        // 这里将会放置D3.js代码来渲染世界地图和添加编码通道
        const container = d3.select('#map-container');

    // 加载SVG文件
    d3.xml('asserts/HighlightLight.svg').then((data) => {
      container.node().append(data.documentElement);

      // 在这里，你可以添加更多D3.js的代码来处理地图
      // 例如，改变国家的颜色，根据数据添加圆点等
    });
      }
    }
  };
  </script>
  