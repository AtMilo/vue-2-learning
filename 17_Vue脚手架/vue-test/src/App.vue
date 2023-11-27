<template>
    <div>
        <h1 v-text="msg" ref="title"></h1>
        <button @click="showDOM()" ref="btn">点我显示DOM</button>
        <SimpSchool id="school" ref="school"></SimpSchool>
        <SimpSchool></SimpSchool>
        <SimpSchool></SimpSchool>
    </div>
</template>

<script>
import SimpSchool from "./components/SimpSchool.vue";
export default {
    name: "App",
    data() {
        return {
            msg: "欢迎来到Vue课堂",
            title: "",
        };
    },
    components: {
        SimpSchool,
    },
    methods: {
        showDOM() {
            console.log("@@@", this.$refs.title);
            console.log("@@@", this.$refs.btn);
            console.log("@@@", this.$refs.school);
            console.log("@@@", document.getElementById("school"));
        },
    },
};
</script>

<style></style>
