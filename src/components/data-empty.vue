<template>
    <div class="v-charts-data-empty">
        <div :style="{height}" class="v-charts-bg">
            <img v-if="flag==='dark'" src="./images/default.png">
            <img v-else src="./images/default-light.png">
            <div class="pt30 ml30 ">
                <p class="f16 ">暂无数据</p>
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

