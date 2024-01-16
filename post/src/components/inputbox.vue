<template>
    <h1>
        Two Way Binding multiple input box
    </h1>
    <h3>Select Sport: {{ hobby }}</h3>
    <label for="">Basket</label>
    &nbsp;
    <input type="checkbox" value="Basket" v-model="hobby" id="" />
    <br />
   <label for="">Footballs</label>
    &nbsp;
    <input type="checkbox" value="Footballs" v-model="hobby" id="" />
    <br />
   <label for="">Fulsals</label>
    &nbsp;
    <input type="checkbox" value="Fulsals" v-model="hobby" id="" />
    <br />

    <h3>Select Player: {{ player }}</h3>
    <label for="">Player Name :</label>
    &nbsp;
    <label for="">Jamal</label>
    <input type="radio" value="Jamal" v-model="player" id="" />
    &nbsp;
    <label for="">Akmal</label>
    <input type="radio" value="Akmal" v-model="player" id="" />
     &nbsp;
    <label for="">Akhi</label>
    <input type="radio" value="Akhi" v-model="player" id="" />
     &nbsp;
    <label for="">Ali</label>
    <input type="radio" value="Ali" v-model="player" id="" />

</template>
<script>
export default {
    name: "input_box",
    data() {
        return {
            hobby: [],
            player: '',
        }
    }

}
</script>
<style>
h1 {
    color: rgb(red, green, blue)
}
</style>