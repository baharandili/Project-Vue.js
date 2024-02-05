<template>
<h1>Form Test</h1>
<form action="">
<lb for="">Username :</lb>&nbsp;
<input type="text" name="" id="" placeholder="Isi Username" v-model="username" />
<p/>
<lb for="">Password :</lb>&nbsp;&nbsp;
<input type="password" name="" id="" placeholder="Isi Password" v-model="password"/> 
<p/>
<lb for="">Email :</lb>&nbsp;&nbsp;
<input type="email" name="" id="" placeholder="Isi Email" v-model="email"/> 
<p/>
<lb for="">No Hp :</lb>&nbsp;&nbsp;
<input type="num" name="" id="" placeholder="Isi Nomor" v-model="nope"/>
<br>
<button v-on:click="login">Sign Up</button>
</form>
<!-- <p> {{ form }}</p> -->
</template>
<script>
export default{
    name: "form_comp",
    data(){
        return{
            form:{
            username: "",
            password: "",
            email: "",
            nope: ""
        }
    }

    },
    methods:{
        login(){
        console.log("Login Data",this.Form);
        }

    }
    }
</script>
<style>
h1{
    color: brown
}
</style>