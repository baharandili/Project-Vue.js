<template>
    <!-- <h1>Test newuser</h1> -->
    <div class="comp">
        <!-- <h2>{{ data[0].name }}</h2> -->
        <!-- <h2>{{ data }}</h2> -->
    </div> 
</template>
<script>
export default{
    name: "new_user",
    props: {
        data: Object,
    }, 
}
</script>
<style>
h1{
    color: black;
}
comp{
    padding: 15px;
    margin-bottom: 20px;
    border: 1px solid;
    background-color: aqua;
}
</style>