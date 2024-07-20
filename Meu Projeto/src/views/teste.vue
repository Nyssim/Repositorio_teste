<script setup>
    import {ref} from 'vue'

    const nome = ref('Ex: Adriano')
    const email = ref('Ex: adriano123@gmail.com')
    const genero = ref('Prefiro não responder')
    const endereco = ref('Ex: QD00 LT00')
    const telefone = ref('Ex: 62912345678')
    const comentario = ref('Ex Gostei da plataforma')
    
</script>

<template>
    <main>
        <h1>Formulario</h1>
        <label>nome</label>
        <input v-model="nome" required> <span> {{ nome }} </span>
        <label>email</label>
        <input v-model="email" type="email" required> {{ email }}
        <label>genero</label>
        <select v-model="genero">
            <option disabled value="">Prefiro não responder</option>
            <option >Masculino</option>
            <option >Feminino</option>
        </select>
        <label>endereco</label>
        <input v-model="endereco"> {{ endereco }}
        <label>telefone</label>
        <input v-model="telefone" type="number"> {{ telefone }}
        <label>Comentarios</label>
        <input v-model="comentario"> <span> {{ comentario }} </span>
    </main>

</template>

<style>

main {
    display: flex;
    width: 100vw;
    height: 90vh;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
}

input {
    width: 25vw;
}

</style>