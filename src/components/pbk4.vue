<script setup>
import { ref } from "vue";
const count =ref(0);
const increment = () => {
    count.value++;
};
const reset = () => {
    count.value =0;
}

</script>

<template>
<div>
    <h1>Klik Tombol</h1>
    <p>Nilai: {{ count }}</p>

    <button @click="increment">Tambah</button>
    <button @click="reset">Reset</button>
</div>
</template>

<style scopped>
button {
    margin-right: 5px;
}

</style>