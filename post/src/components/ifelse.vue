<template>
    <h1 v-if="display">Tutor dek if</h1>
    <h1 v-else>Tutor dek else </h1>
    <button v-on:click="display = !display">Click Here</button>
</template>
<script>
export default {
    name: "ifElse",
    data() {
        return {
            display:true,
            show:false,

        }
    }

}
</script>
<style>
h1 {
    color: rgb(red, green, blue)
}
</style>