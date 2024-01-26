<template>
<h3>Dosen {{ name }}</h3>
<button v-on:click="getUserName(userName)">Check The Name </button>
</template>
<script>
export default{
    name: "dosen_com",
    props: {
        name:String,
        getUserName: Function
    }, 
    data(){
        return{
            userName: "Jamal",
        }
    }
}
</script>