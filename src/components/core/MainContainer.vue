<template>
    <div class="ph-main-container">
        <img src="../../assets/images/modulo_salud.png" alt="Ejemplo de Módulo de Salud de Phoenix">
    </div>
</template>

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