<template>
    <!-- <h1>Awas Sedang Test Child</h1> -->
    <!-- <h3>{{ name }}</h3> -->
    <!-- <h3>{{ users.name }}</h3>
    <h3>{{ users.email }}</h3>
    <button v-on:click="getData()"> Click Disini Yaa </button> -->
       <!-- <ul>
        <li v-for="item in user" :key="item.name"> 
            {{ item.name }} ,
            {{ item.email }} 
            <h2>{{ item.name }}</h2>
            <h2>{{ item.email }}</h2>
            <Newuser :data="item"/>
        </li>
    </ul>
    <div>
    <h1 v-html="emls"></h1>
    <div v-html="id"></div>
    </div> -->
    <h3 :class="{aqua:color}">Class Dynamic</h3>
    <button v-on:click="color=!color">Click Here</button>
    <Newuser/>
</template>
<script>
import Newuser from './newuser.vue';
export default {
    name: "childs_com",
    props: {
        name: String,
        user: Object,
        getData: Function,
    },
    data() {
        return {
            // user: [
            //     {
            //         name: 'Jaks',
            //         email: 'jamali1@gmail.com'
            //     },
            //     {
            //         name: 'Jams',
            //         email: 'jamali2@gmail.com'
            //     },
            //     {
            //         name: 'Joks',
            //         email: 'jamali3@gmail.com'
            //     },
            //     {
            //         name: 'Kaml',
            //         email: 'jamali4@gmail.com'
            //     },
            //     {
            //         name: 'yogs',
            //         email: 'jamali5@gmail.com'
            //     }
            // ]
            // names:'jamal',
            // emls:'<h3>jams3@gmail.com</h3>',
            // id: 82244770086,
            color :false
        };
    },
    
    components: { Newuser }
};
</script>
<style>
.aqua{
    color:blue;
    font-weight: bold;
    background-color: aqua;
    border-color: black;
    width: 160px;
    height: 20px;
}
</style>