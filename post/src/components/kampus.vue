<template>
    <!-- <h3>{{ childUser }}</h3> -->
    <h3>Main Kampus</h3>
    <Dosen name="Bahar" :getUserName="getUserName"/>
    <Mahasiswa name="Andi" :getUserName="getUserName"/>
</template>
<script>
// import Dosen1 from './dosen.vue';
import Dosen from './dosen.vue';
import Mahasiswa from './mahasiswa.vue';
export default {
    name: "kampus_com",
    methods: {
        getUserName(name){
        alert(name)
        // this.childUser = (name);
        },
    // data(){
    //     return{
    //         childUser:"",
    //     }
    // }
    },
    components: { Mahasiswa, Dosen }
}
</script>