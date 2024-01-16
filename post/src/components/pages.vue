<template>
    <h1>
        Two Way Binding
    </h1>
    <input type ="text" placeholder=" " v-model="name"/>
    <h3>{{ name }}</h3>
</template>
<script>
  export default {
    name: "pages_One",
    data(){
        return{
            name: this.name,
        }
    }
 
}
</script>
<style>
h1{
    color:rgb(red, green, blue)
}
</style>