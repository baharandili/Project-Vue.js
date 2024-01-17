<template>
    <!-- <h1>Awas Sedang Test Child</h1> -->
    <!-- <h3>{{ name }}</h3> -->
    <!-- <h3>{{ users.name }}</h3>
    <h3>{{ users.email }}</h3>
    <button v-on:click="getData()"> Click Disini Yaa </button> -->
    <Newuser />
    <ul>
        <li v-for="item in user" :key="item.name"> 
            <!-- {{ item.name }} ,
            {{ item.email }}  -->
            <Newuser :data="item"/>
        </li>
    </ul>
</template>
<script>
import Newuser from './newuser.vue';
export default {
    name: "childs_com",
    props: {
        name: String,
        users: Object,
        getData: Function,
    },
    data(){
        return{
            user:[
                {
                name:'Jaks',
                email:'jamali1@gmail.com'
            },
            {
                name:'Jams',
                email:'jamali2@gmail.com'
            },
            {
                name:'Joks',
                email:'jamali3@gmail.com'
            },
            {
                name:'Kaml',
                email:'jamali4@gmail.com'
            },
            {
                name:'yogs',
                email:'jamali5@gmail.com'
            }
        ]
        }
    },
    components: { Newuser }
};
</script>
<style>
h3{
    color:aqua,
}
</style>