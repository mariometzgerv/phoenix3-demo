<template>
    <nav class="navbar navbar-expand-lg fixed-top shadow-lg ph-secondary ph-topbar">
        <div class="container">
            <button class="navbar-toggler hidden-lg-up navbar-toggler-icon" type="button" data-bs-toggle="collapse" data-bs-target="#collapsibleNavId" aria-controls="collapsibleNavId" aria-expanded="false" aria-label="Toggle navigation"></button>
            
            <div class="collapse navbar-collapse" id="collapsibleNavId">
                <div class="col">
                    <div class="container">
                        <img src="../../assets/images/logo_uls_chile.png" alt="Logo Universidad de La Serena" height="50px">
                    </div>
                </div>

                <div class="col-2">
                    <div class="container">
                        <button type="button" class="btn ph-primary ph-primary-text ph-btn">
                            <i class="fa fa-universal-access"></i>
                            Accesabilidad
                        </button>
                    </div>
                </div>

                <div class="col-4">
                    <div class="container input-group">
                        <span class="input-group-text border-0 ph-primary ph-secondary-text ph-btn-no-border"><i class="fa fa-search"></i></span>
                        <input type="search" class="form-control border-0 ph-primary ph-primary-text" placeholder="Buscar" aria-label="Buscar">
                        <button type="button" class="btn ph-primary ph-secondary-text ph-btn-no-border">
                            <i class="fa fa-microphone"></i>
                        </button>
                    </div>
                </div>

                <div class="col">
                    <div class="container">
                        <button type="button" class="btn ph-secondary ph-primary-text ph-btn-no-border ph-icon">
                            <i class="fa fa-bell"></i>
                        </button>
                    </div>
                </div>
                
                <div class="col-3">
                    <div class="container">
                        <button type="button" class="btn ph-secondary ph-primary-text ph-btn">
                            <img src="../../assets/images/perfil.png" alt="Logo Universidad de La Serena" height="50px">
                            Nombre_Estudiante
                        </button>
                    </div>
                </div>

                <div class="col">
                    <div class="ph-log-out">
                        <button type="button" class="btn ph-secondary ph-primary-text ph-btn"  @click="menu_visible = !menu_visible">
                            <i class="fa fa-ellipsis-v"></i>
                        </button>
                    </div>

                    <div v-show="menu_visible">
                        <MenuSettings/>
                    </div>
                </div>
            </div>
        </div>
    </nav>

    <div style="height: 80px;"></div>
</template>

<script>
    import MenuSettings from './MenuSettings.vue';

    export default
    {
        name: 'TopBar',
        components: {
            MenuSettings
        },
        data: function () {
            return {
                menu_visible: false
            };
        }
    }
</script>

<style scoped>
    i
    {
        font-size: 24px;
    }
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
    .ph-topbar
    {
        animation: 1s ease-out 0s 1 slide-top;
    }
    .ph-log-out {
        position: fixed;
        top: 16px;
        right: 16px;
    }
</style>
