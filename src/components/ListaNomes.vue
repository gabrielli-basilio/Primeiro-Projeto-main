<script setup>
import { ref } from 'vue'

const nomeNovo = ref('')

const nomes = ref(['Eduardo', "Matheus", "Gabriel"])


function adicionar(){
    nomes.value.push(nomeNovo.value)
    nomeNovo.value = ''
}
</script>

<template>
    <section>
        <h2>Lista de nomes</h2>

        <input type="text" v-model="nomeNovo">
        <button @click="adicionar">Adicionar</button>

        <ul>
            <li v-for="nome in nomes" :key="nome">
                {{ nome }}
            </li>
        </ul>
    </section>
</template>