<script setup>
    defineProps({
        nome: String,
        curso: String
    })
</script>

<template>
    <section>
        <h2>Pessoa</h2>
        <p><strong>Nome: </strong> {{ nome }} </p>
        <p><strong>Curso: </strong> {{ curso }}</p>
    </section>
</template>

<style scoped>
    section{
        background: white;
        padding: 20px;
        border-radius: 10px;
        box-shadow: 0 5px 5px 0 rgb(0, 0, 0, 0.3);
    }
</style>