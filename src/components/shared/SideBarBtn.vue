<template>
    <td rowspan="1" colspan="1" v-if="tipo == 1">
        <button type="button" class="btn p-2 ph-bg ph-primary-text ph-modulo-icono ph-btn-zoom">
            <img v-bind:src="icono" alt="Botón" width="32">
        </button>
    </td>
    <td rowspan="2" colspan="2" v-if="tipo == 2">
        <button type="button" class="btn p-2 ph-bg ph-primary-text ph-modulo-icono ph-btn-zoom">
            <img v-bind:src="icono" alt="Botón" width="64">
            <div>Servicio Salud</div>
        </button>
    </td>
    <td rowspan="1" colspan="3" v-if="tipo == 3">
        <button type="button" class="btn p-2 ph-bg w-100 text-start ph-primary-text ph-modulo-icono ph-btn-zoom">
            <img v-bind:src="icono" alt="Botón" width="32">
            Deportes
        </button>
    </td>
</template>

<script>
export default
{
    name: 'SideBarBtn',
    props:
    {
        icono: String,
        tipo: Number
    }
}
</script>

<style scoped>
    .ph-modulo-icono {
        border-radius: 15px;
        transition-duration: 0.5s;
    }
    .ph-modulo-icono:hover {
        border-color: #FFFFFF;
    }
</style>
