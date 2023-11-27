<template>
    <!-- 组件的结构 -->
    <div class="demo">
        <h2>学校名称：{{ schoolName }}</h2>
        <h2>学校地址：{{ schoolAddress }}</h2>
        <button @click="showName">点我显示学校名称</button>
    </div>
</template>

<style>
/* 组件的样式 */
.demo {
    background-color: #ab5;
    border-radius: 10px;
}
</style>

<script>
// 组件的交互相关代码
export default {
    name: "School",
    data() {
        return {
            schoolName: "浙大",
            schoolAddress: "浙江杭州",
        };
    },
    methods: {
        showName() {
            alert(this.schoolName);
        },
    },
};
</script>
