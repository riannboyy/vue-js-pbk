<script setup>
 import { ref } from "vue";
 const name = ref("Adra");
 const age = ref ("19");
</script>

<template>
 <div class="container">
  <h1>Tugas Pertemuan 4 PBK</h1>
  <p>Halo, Nama Saya {{ name }} dan saya berumur{{ age }}tahun.</p>
 </div>

</template>

<style scopped>
.container {
    text-align: center;
    margin-top: 50px;
}   
h1 {
    color: rgb(239, 8, 8);
    font-size: 25px;
    font-weight: bold;
}
</style>