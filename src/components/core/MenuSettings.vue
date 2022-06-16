<template>
    <div class="container ph-primary-text ph-panel ph-bg">
        <div class="d-flex flex-column flex-shrink-0 p-3">
        <a href="/" class="d-flex align-items-center mb-3 mb-md-0 me-md-auto text-white text-decoration-none">
        <span class="fs-4">Menú</span>
        </a>
        <hr>
        <ul class="nav nav-pills flex-column mb-auto">
            <li class="nav-item">
                <a href="#" class="nav-link text-white" aria-current="page">
                    Opciones
                </a>
            </li>
            <li>
                <a href="#" class="nav-link text-white">
                    Estadísticas
                </a>
            </li>
            <li>
                <a href="#" class="nav-link text-white">
                    Logros
                </a>
            </li>
            <li>
                <a href="#" class="nav-link text-white">
                    Información
                </a>
            </li>
            <li>
                <a href="#" class="nav-link text-white">
                    Ayuda
                </a>
            </li>
        </ul>
        <hr>
        <a href="#" class="nav-link text-white">
            Cerrar Sesión
        </a>
        </div>
    </div>
</template>

<style scoped>
    @keyframes slide-top
    {
        0%
        {
            transform: translateY(-100%);
        }
        100%
        {
            transform: translateY(0);
        }
    }
    .ph-panel {
        position: absolute;
        width: 300px;
        right: 30px;
        border-radius: 15px;
        animation: 0.5s ease-out 0s 1 slide-top;
    }
</style>