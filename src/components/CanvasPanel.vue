<template>
    <div class="Panel-Border">
        <div class="Panel-Title">
            Canvas Panel
        </div>
        <div class="Panel-Content">
            
            <img v-if="selectedImage" :src="selectedImage" />
        </div>
    </div>
</template>
  
    
<script>
export default {
  props: ['selectedImage']
}
</script>
    
<style scoped>
.Panel-Title {
    background-color: #D9D9D9;
    width: fit-content;
}
.Panel-Border {
    width: 100%;
    height: 100%;
    border: 4px solid #D9D9D9;
    
}

.Panel-Content {
    width: 100%; /* 确保 Panel-Content 占满父容器的宽度 */
    height: 100%; /* 确保 Panel-Content 占满父容器的高度 */
    display: flex; /* 使用 flex 布局使内容居中 */
    justify-content: center; /* 水平居中图片 */
    align-items: center; /* 垂直居中图片 */
}

.Panel-Content img {
    width: 100%; /* 图片占满 Panel-Content 的宽度 */
    height: 100%; /* 图片占满 Panel-Content 的高度 */
    object-fit: contain; /* 调整图片的填充方式为contain，避免图片失真 */
}
</style>
    