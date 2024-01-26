<template>
<h3>Mahasiswa {{ name }}</h3>
<button v-on:click="getUserName(userName)">Click Here</button>
</template>
<script>
export default{
    name: "mahasiswa_com",
    props:{
        name:String,
        getUserName: Function,
    },
    data(){
        return{
        userName:"akhmad",
        }
    }   
}
</script>
<style>
h3{
    color: blueviolet;
}
</style>