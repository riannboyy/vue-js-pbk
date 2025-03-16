<script setup>
import { ref } from "vue";

const count= ref(0);

const increment = () => {
    count.value++;
}
</script>

<template>
<div class="container"> 
    <h1>Adra Herlyan</h1>
    <p> Nilai: {{ count }}</p>
    <button @click="increment">Tambah</button>
</div>

</template>

<style scopped>
.container {
    text-align: center;
    margin-top: 55px;
}
button {
    padding: 10px 20px;
    font-size: 20px;
    cursor: pointer;
    background-color: aquamarine;
    color: white;
    border: none;
    border-radius: 5px;
}

</style>