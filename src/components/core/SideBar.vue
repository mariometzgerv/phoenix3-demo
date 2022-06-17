<template>
    <div class="d-flex bd-highlight">
        <div class="col-2">
            <div class="d-flex flex-column flex-shrink-0 p-3 ph-primary-text ph-primary ph-sidebar">
                <hr>
                <a href="#" class="d-flex align-items-center text-decoration-none">
                    <span class="ph-secondary-text">FAVORITOS</span>
                    <div class="w-100 text-end">
                        <button type="button" class="btn ph-secondary-text ph-btn" @click="favoritos_visible = !favoritos_visible">
                            <i class="fa fa-chevron-down"></i>
                        </button>
                    </div>
                </a>
                <hr>

                <div class="table-responsive ph-collapsable" v-show="favoritos_visible">
                    <table>
                        <tr>
                            <SideBarBtn @modulo="modulo = 1" :tipo=2 :icono="require(`@/assets/${'images/iconos-modulos/servicio_salud.png'}`)"/>
                            <SideBarBtn @modulo="modulo = 2" :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/comunicaciones.png'}`)"/>
                            <SideBarBtn @modulo="modulo = 3" :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/registro.png'}`)"/>
                            <SideBarBtn @modulo="modulo = 4" :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/soporte.png'}`)"/>
                        </tr>
                        <tr>
                            <SideBarBtn @modulo="modulo = 5" :tipo=3 :icono="require(`@/assets/${'images/iconos-modulos/deportes.png'}`)"/>
                        </tr>
                    </table>
                </div>

                <hr>
                <a href="#" class="d-flex align-items-center text-decoration-none">
                    <span class="ph-secondary-text">APLICACIONES</span>
                    <div class="w-100 text-end">
                        <button type="button" class="btn ph-secondary-text ph-btn" @click="aplicaciones_visible = !aplicaciones_visible">
                            <i class="fa fa-chevron-down"></i>
                        </button>
                    </div>
                </a>
                <hr>

                <div class="table-responsive ph-collapsable" v-show="aplicaciones_visible">
                    <table>
                        <tr>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-aplicaciones/gmail.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-aplicaciones/gmeet.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-aplicaciones/zoom.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-aplicaciones/moodle.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-aplicaciones/gclassroom.png'}`)"/>
                        </tr>
                    </table>
                </div>  

                <hr>
                <a href="#" class="d-flex align-items-center text-decoration-none">
                    <span class="ph-secondary-text">MÓDULOS</span>
                    <div class="w-100 text-end">
                        <button type="button" class="btn ph-secondary-text ph-btn" @click="modulos_visible = !modulos_visible">
                            <i class="fa fa-chevron-down"></i>
                        </button>
                    </div>
                </a>
                <hr>

                <div class="table-responsive ph-collapsable" v-show="modulos_visible">
                    <table>
                        <tr>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/soporte.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/deportes.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/servicio_salud.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/comunicaciones.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/registro.png'}`)"/>
                        </tr>
                        <tr>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/servicio_salud.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/comunicaciones.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/deportes.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/soporte.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/deportes.png'}`)"/>
                        </tr>
                        <tr>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/deportes.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/registro.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/servicio_salud.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/comunicaciones.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/soporte.png'}`)"/>
                        </tr>
                        <tr>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/servicio_salud.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/comunicaciones.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/registro.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/soporte.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/deportes.png'}`)"/>
                        </tr>
                        <tr>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/servicio_salud.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/comunicaciones.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/deportes.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/soporte.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/deportes.png'}`)"/>
                        </tr>
                        <tr>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/deportes.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/registro.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/servicio_salud.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/comunicaciones.png'}`)"/>
                            <SideBarBtn :tipo=1 :icono="require(`@/assets/${'images/iconos-modulos/soporte.png'}`)"/>
                        </tr>
                    </table>
                </div>
                <hr>

                <div class="w-100 text-end">
                    <button type="button" class="btn ph-secondary-text ph-btn">
                        <i class="fa fa-chevron-left"></i>
                    </button>
                </div>
            </div>
        </div>
        <div>
            <MainContainer :modulo="modulo" />
        </div>
    </div>
</template>

<script>
    import SideBarBtn from './../shared/SideBarBtn.vue';
    import MainContainer from './MainContainer.vue';

    export default {
        name: 'SideBar',
        components: {
            SideBarBtn,
            MainContainer
        },
        data: function () {
            return {
                favoritos_visible: true,
                aplicaciones_visible: true,
                modulos_visible: true,
                modulo: 1
            };
        }
    };
</script>

<style scoped>
    @keyframes slide-top {
        0% {
            transform: translateY(-100%);
        }
        100% {
            transform: translateY(0);
        }
    }
    @keyframes slide-left {
        0% {
            transform: translateX(-100%);
        }
        100% {
            transform: translateX(0);
        }
    }
    .ph-sidebar {
        animation: 1s ease-out 0s 1 slide-top;
    }
    .ph-collapsable {
        animation: 0.5s ease-out 0s 1 slide-left;
    }
</style>
