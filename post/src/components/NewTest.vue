<template>
    <!-- <h1>HAI</h1> -->
    <h1>Email : {{ email }}</h1>
    <h1>nope : {{ nope }}</h1>
    <h1>name : {{ getName("Jams") }}</h1>
    <h1>name 2 : {{ getName("jamal") }}</h1>
    <h1>Data : {{ getData().email }}</h1>
    <h1>Data : {{ getData().Phone }}</h1>
    <button v-on:click="func()"> Click Here </button>
    <h1 v-on:mousemove="getConsole()">Home</h1>
    <!-- <h1>name {{ "jamal" }}</h1> -->
</template>
<script>
export default{
    name:"PAGES",
    data(){
        return{
            email: "abs@abs.com",
            nope: "88888",
            // name1: function(a){
            //     return a;
            // }
        };
    },
    methods: {
        getName(name){
            return name;
        },
        getData(){
            return{
            email: this.email,
            Phone: this.nope,
            }
        },
        func(){
            alert("hai ges")
        },
        getConsole(){
            console.warn("Function Was Running")
        },
    },
};
</script>
<style scoped>
h1{
    color :blue
}
</style>
