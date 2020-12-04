<template>
    <div class="v-charts-data-empty">
        <div :style="{height}" class="v-charts-bg">
            <img :src="require('../images/default-light.png')">
            <div class=" pt30 ml30 ">
                <p class=" f16 ">暂无数据</p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props: {
        flag: String,
        height: String
    },

};
</script>
<style scoped>
    .v-charts-data-empty {
        position: absolute;
        left: 0;
        right: 0;
        top: 0;
        bottom: 0;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: rgba(255, 255, 255, 0.7);
        color: #888;
        font-size: 14px;
        z-index: 999;
    }
    .f16 {
        padding-top: 30px;
        margin-left: 30px;
        font-size: 16px;
        color: #a0a3a8;
    }
    .v-charts-bg {
        display: flex;
        justify-items: center;
        align-items: center;
    }
</style>

