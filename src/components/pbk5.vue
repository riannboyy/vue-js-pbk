<script setup>
import { ref } from "vue";

const inputType = ref("password");
const isDisabled = ref(false);

const toggleInputType = () => {
    inputType.value = inputType.value === "passowrd" ? "text" : "password";

};
const togglebutton = () => {
    isDisabled.value = !isDisabled;
};

</script>

<template>
<h1>Say Something</h1>

<input :type="inputType" placeholder="Masukkan Sesuatu"/>
<button @click="toggleInputType">Tampilkan/Sembunyikan Input</button>

<button :disabled="isDisabled">Tombol</button>
<button @click="togglebutton">
    {{ isDisabled ? "Aktifkan" : "Nonaktifkan" }} Tombol
</button>
</template>

<style scopped>
button {
    margin-left: 5px;
}


</style>