<template>
    <!-- <h1 id="pages3">Tutor loops ni bos</h1> -->
    <ul>
        <li v-for="program in technology" :key="program">
            {{ technology }}
        </li>
    </ul>
    <br>
    <!-- <ul>
        <li v-for="data in user" :key="data">name: {{ data.name }}</li>
        <li v-for="data in user" :key="data">email: {{ data.email }}</li>
        <li v-for="data in user" :key="data">contact: {{ data.contact }}</li>
    </ul> -->
    <Childs name="Bahar Andili yakan" :user="user" :getData="getData" />
</template>
<script>
import Childs from './childs.vue';
export default {
    name: "for_loops",
    // data() {
    //     return {
    //         technology: ["PHP", "C#", "C++", "Java", "Python"],
    //         user: [
    //             {
    //                 name: "Jaks",
    //                 email: "Jaks@gmail.com",
    //                 contact: +9456423720
    //             },
    //             {
    //                 name: "Jamal",
    //                 email: "Jamal@gmail.com",
    //                 contact: +945644678
    //             },
    //             {
    //                 name: "Joms",
    //                 email: "Joms@gmail.com",
    //                 contact: +945646542
    //             },
    //         ]
    //     };
    // },
    // data(){
    //     return{
    //     user:{ name:"jamal", email:"bahar@gmail.com" },
    //     }
    // },
    methods:{
        getData(){
            alert("Pante Kau, Hehehehe ")
        }

    },
    components: { Childs }
}
</script>
<style>
#pages3 {
    color: blue
}
</style>