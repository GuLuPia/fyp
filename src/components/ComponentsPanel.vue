<template>
  <div class="Panel-Border">
    <div class="Panel-Title">
      Components Panel
    </div>
    <div class="Components-Panel-Layout">
      <div id="Highlight">
        <!-- 监听子组件发射的image-selected事件 -->
        <Highlight-Techniques @image-selected="handleImageSelected"/>
      </div>

      <div id="EncodingChannels">
        <Encoding-Channels />
      </div>

      <div id="BasicMapRepresentation">
        <Basic-Map-Representation />
      </div>

      <div id="MapProjections">
        <Map-Projections />
      </div>

      <div id="LabelPositions">
        <Label-Positions />
      </div>

      <div id="CanvasPanel">
        <!-- 将选中的图片传递给CanvasPanel组件 -->
        <Canvas-Panel :selectedImage="selectedImage"/>
      </div>
    </div>
  </div>
</template>

<script>
import HighlightTechniques from './HighlightTechniques.vue'
import EncodingChannels from './EncodingChannels.vue'
import MapProjections from './MapProjections.vue'
import BasicMapRepresentation from './BasicMapRepresentation.vue'
import LabelPositions from './LabelPositions.vue'
import CanvasPanel from './CanvasPanel.vue';

export default {
  components: {
    'Highlight-Techniques': HighlightTechniques,
    'Encoding-Channels': EncodingChannels,
    'Map-Projections': MapProjections,
    'BasicMapRepresentation': BasicMapRepresentation,
    'LabelPositions': LabelPositions,
    'Canvas-Panel': CanvasPanel
  },
  data() {
    return {
      selectedImage: null // 用于存储被选中的图片路径
    };
  },
  methods: {
    handleImageSelected(imageSrc) {
      this.selectedImage = imageSrc; // 更新selectedImage为被选中的图片路径
    }
  }
}
</script>

  
<style>
.Dimension-Title {
  margin-top: 7px;
  padding: 4px;
  font-size: 18px;
  border-radius: 7px;
  display: block;
  width: fit-content;
}

.Dimension-Border {
  clear: both;
  border: 2px solid;

  height: 100%;
  width: 100%;

  display: flex;
  justify-content: center;
  align-items: center;
}

.Dimension-Layout {
  display: grid;
  gap: 6px;
}

.element {
  display: inline-block;
  text-align: center;
  margin-top: 5px;
  font-size: 12px;

  /* 设置图片的初始样式 */
  border: 4px solid transparent;
  /* 用透明边框占位，避免悬停时改变尺寸 */
  transition: border-color 0.3s;
  /* 平滑过渡效果 */
}

.element:hover {
  /* 定义鼠标悬停时的样式 */
  border-color: rgba(255, 0, 0, 0.3);
  /* 边框颜色变为红色 */
}

.element:active {
  border-color: rgba(255, 0, 0, 0.9);
}

.element img {
  display: block;
  margin-top: 3px;
}

.layout {
  width: 100%;
  height: 100%;

  display: flex;
  flex-direction: column;
}

.Components-Panel-Layout {
  /* display: flex;
  flex-wrap: wrap;  */
  display: grid;
  width: fit-content;
  height: fit-content;

  gap: 15px;
  margin: 15px
}

.img {
  display: flex;
  justify-content: center;
  align-items: center;
}

#Highlight {
  grid-column: 1 / 2;
  grid-row: 1 / 4;
}

#EncodingChannels {
  grid-column: 2 / 3;
  grid-row: 1 / 2;
}

#MapProjections {
  grid-column: 3 / 4;
  grid-row: 1 / 2;
}

#BasicMapRepresentation {
  grid-column: 2 / 4;
  grid-row: 2 / 3;
}

#LabelPositions {
  grid-column: 1 / 2;
  grid-row: 4 / 5;
}

#CanvasPanel {
  grid-column: 2 / 4;
  grid-row: 3 / 5;
}</style>