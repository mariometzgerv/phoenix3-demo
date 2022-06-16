<template>
    <TopBar/>

    <div class="d-flex bd-highlight">
        <div class="col-2">
            <SideBar/>
        </div>
        <div>
            <MainContainer/>
        </div>
    </div>
</template>

<script>
    import TopBar from './components/core/TopBar.vue';
    import SideBar from './components/core/SideBar.vue';
    import MainContainer from './components/core/MainContainer.vue';

    export default
    {
        name: 'App',
        components:
        {
            TopBar,
            SideBar,
            MainContainer
        }
    }
</script>

<style>
    .ph-bg {
        background-color: #00004A;
    }
    .ph-primary {
        background-color: #00007A;
    }
    .ph-secondary {
        background-color: #0000A3;
    }
    .ph-secondary-text {
        color: #808080;
    }
    .ph-btn,
    .ph-btn-no-border {
        transition-duration: 0.5s;
    }
    .ph-icon:hover i {
        transition-duration: 0.1s;
    }
    .ph-btn:hover {
        border-color: #FFFFFF;
        color: #FFFFFF;
    }
    .ph-btn-no-border:hover,
    .ph-primary-text,
    .ph-primary-text:hover {
        color: #FFFFFF;
    }
    .ph-icon:hover i {
        font-size: 32px;
    }
    button {
        opacity: 0;
        animation: zoom 2s ease forwards;
    }
    @keyframes zoom {
        0% {
            opacity: 0
        }
        100% {
            opacity: 1
        }
    }
</style>
