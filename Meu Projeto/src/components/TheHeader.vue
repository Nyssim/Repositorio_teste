<script setup lang="ts">
    import { RouterLink, RouterView } from 'vue-router'
    import '../assets/header.css'
</script>


<template>
    <header>
        <img src="https://img.freepik.com/vetores-gratis/modelo-de-logotipo-de-sabao_23-2148706677.jpg" alt="Logotipo de teste">
        <nav>
            <div id="rotas">
                <RouterLink to="/">Home</RouterLink>
                <RouterLink to="/about">About</RouterLink>
                <RouterLink to="/Ladding_page">Pagina Inicial</RouterLink>
            </div>
        </nav>
    </header>
    <RouterView />
</template>