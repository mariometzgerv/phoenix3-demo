<template>
    <TopBar/>
    <SideBar/>
</template>

<script>
import TopBar from './components/core/TopBar.vue'
import SideBar from './components/core/SideBar.vue'

export default {
    name: 'App',
    components: {
        TopBar,
        SideBar
    }
}
</script>
