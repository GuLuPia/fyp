<template>
    <div class="layout">
        <div class="Dimension-Title">
            <div>Highlight Techniques</div>
        </div>

        <div class="Dimension-Border">
            <div class="Dimension-Layout">
                <div class="element" id="Light" @click="handleClick('HighlightLight')">
                    Light
                    <div class="img"><img src="../assets/HighlightLight.svg" /></div>
                </div>

                <div class="element" id="Color" @click="handleClick('HighlightColor')">
                    Color
                    <div class="img"><img src="../assets/HighlightColor.svg" /></div>
                </div>

                <div class="element" id="Map-Pin" @click="handleClick('HighlightMappin')">
                    Map Pin
                    <div class="img"><img src="../assets/HighlightMappin.svg" /></div>
                </div>

                <div class="element" id="3D-Transformation" @click="handleClick('Highlight3d')">
                    3D Transformation
                    <div class="img"><img src="../assets/Highlight3d.svg" /></div>
                </div>
                <div class="element" id="Enlarged-Portions" @click="handleClick('HighlightEnlarge')">
                    Enlarged Portions
                    <div class="img"><img src="../assets/HighlightEnlarge.svg" /></div>
                </div>
            </div>

        </div>
    </div>
</template>
    

<script>
// 引入图片
import HighlightLight from '../assets/HighlightLight.svg';
import HighlightColor from '../assets/HighlightColor.svg';
import HighlightMappin from '../assets/HighlightMappin.svg';
import Highlight3d from '../assets/Highlight3d.svg';
import HighlightEnlarge from '../assets/HighlightEnlarge.svg';

export default {
  methods: {
    handleClick(imageName) {
      // 根据传入的imageName决定发射哪个图片的路径
      const images = {
        HighlightLight,
        HighlightColor,
        HighlightMappin,
        Highlight3d,
        HighlightEnlarge
      };
      this.$emit('image-selected', images[imageName]);
    }
  }
}
</script>

    
<style scoped>
.Dimension-Border {
    border-color: #74BBAA;

}

.Dimension-Title {
    background-color: #74BBAA;
}

#Light {
    grid-row: 1 / 2;
    grid-column: 1 / 2;
}

#Color {
    grid-row: 1 / 2;
    grid-column: 2 / 3;
}

#Map-Pin {
    grid-row: 2 / 3;
    grid-column: 1 / 2;
}

#3D-Transformation {
    grid-row: 2 / 3;
    grid-column: 2 / 3;
}

#Enlarged-Portions {
    grid-row: 3 / 4;
    grid-column: 1 / 3;
}
</style>
    