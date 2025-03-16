<script setup>
import { ref } from "vue";

const name = ref("");
const age = ref(null);
const gender= ref("");

</script>

<template>
<div>
    <h1> Masukan Dibawah ini</h1>

    <label>Nama: <input type='text' v-model="name"/></label>
    <label>Umur: <input type='number' v-model="age"/></label>

    <label>
        <input type="radio" value="laki-laki" v-model="gender"/> Laki-laki
    </label>
    <label>
        <input type="radio" value="perempuan" v-model="gender"/> Perempuan
    </label>

    <h2>Hasil:</h2>
    <p>Nama: {{ name }}</p>
    <p>Umur: {{ age }}</p>
    <p>Jenis Kelamin: {{ gender }}</p>
</div>
</template>

<style scopped>
label {
    display: block;
    margin-bottom: 5px;
}

</style>