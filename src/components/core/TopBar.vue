<template>
    <nav class="navbar navbar-expand-lg navbar-light fixed-top shadow-lg ph-bg">
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
                        <button type="button" class="btn ph-primary ph-primary-text">
                            <i class="fa fa-universal-access"></i>
                            Accesabilidad
                        </button>
                    </div>
                </div>

                <div class="col-4">
                    <div class="container input-group">
                        <span class="input-group-text border-0 ph-primary ph-secondary-text"><i class="fa fa-search"></i></span>
                        <input type="search" class="form-control border-0 ph-primary ph-primary-text" placeholder="Buscar" aria-label="Buscar">
                        <button type="button" class="btn ph-primary ph-secondary-text">
                            <i class="fa fa-microphone"></i>
                        </button>
                    </div>
                </div>

                <div class="col">
                    <div class="container">
                        <button type="button" class="btn ph-bg ph-primary-text">
                            <i class="fa fa-bell"></i>
                        </button>
                    </div>
                </div>
                
                <div class="col-3">
                    <div class="container">
                        <button type="button" class="btn ph-bg ph-primary-text">
                            <img src="../../assets/images/perfil.png" alt="Logo Universidad de La Serena" height="50px">
                            Nombre_Estudiante
                        </button>
                    </div>
                </div>

                <div class="col">
                    <div class="container">
                        <button type="button" class="btn ph-bg ph-primary-text">
                            <i class="fa fa-ellipsis-v"></i>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </nav>
</template>

<style scoped>
    .ph-bg
    {
        background-color: #0000A3;
    }
    .ph-primary
    {
        background-color: #00007A;
    }
    .ph-primary-text
    {
        color: #FFFFFF;
    }
    .ph-secondary-text
    {
        color: #808080;
    }
    i
    {
        font-size: 24px;
    }
</style>
