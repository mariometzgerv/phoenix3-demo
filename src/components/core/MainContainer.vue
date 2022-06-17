<template>
    <div class="ph-main-container" v-if="modulo == 1">
        <img src="../../assets/images/modulos/1.png" alt="Ejemplo de Módulo de Salud de Phoenix">
    </div>
    <div class="ph-main-container" v-if="modulo == 2">
        <img src="../../assets/images/modulos/2.png" alt="Ejemplo de Módulo de Salud de Phoenix">
    </div>
    <div class="ph-main-container" v-if="modulo == 3">
        <img src="../../assets/images/modulos/3.png" alt="Ejemplo de Módulo de Salud de Phoenix">
    </div>
    <div class="ph-main-container" v-if="modulo == 4">
        <img src="../../assets/images/modulos/4.png" alt="Ejemplo de Módulo de Salud de Phoenix">
    </div>
    <div class="ph-main-container" v-if="modulo == 5">
        <iframe src="http://localhost/phoenix3/" height="700" width="1000"></iframe>
    </div>
</template>

<script>
    export default {
        name: 'MainContainer',
        props:
        {
            modulo: Number
        }
    };
</script>

<style scoped>
    img
    {
        max-width: 100%;
    }
    @keyframes slide-right
    {
        0%
        {
            transform: translateX(100%);
        }
        100%
        {
            transform: translateX(0);
        }
    }
    .ph-main-container
    {
        animation: 1s ease-out 0s 1 slide-right;
    }
</style>