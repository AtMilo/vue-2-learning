<template>
    <!-- 组件的结构 -->
    <div class="school">
        <h2>学校名称：{{ schoolName }}</h2>
        <h2>学校地址：{{ schoolAddress }}</h2>
    </div>
</template>

<script>
export default {
    data() {
        return {
            schoolName: "浙江大学",
            schoolAddress: "浙江·杭州",
        };
    },
};
</script>

<style>
.school {
    background-color: gray;
}
</style>
