<template>
    <!-- <h1>Awas Sedang Test Child</h1> -->
    <!-- <h3>{{ name }}</h3> -->
    <!-- <h3>{{ user.name }}</h3> -->
    <!-- <h3>{{ user.email }}</h3> -->
    <button v-on:click="getData()"> Click Disini Yaa </button>
    <!-- <Newuser /> -->
</template>
<script>
// import Newuser from './newuser.vue';

export default {
    name: "childs_com",
    props: {
        name: String,
        user: Object,
        getData: Function,
    },
    data(){
        return{

        }
    },
    // components: { Newuser }
};
</script>
<style>
h3{
    color:aqua,
}
</style>