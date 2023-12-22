<script>
import AppMainMenu from './AppMainMenu.vue';
export default {
    name: 'AppMain',
    components: {
        AppMainMenu,
    }

} 
</script>
<template><main>
    <AppMainMenu></AppMainMenu>

</main>
</template>
<style lang="scss" scoped>
main{
    height: 300px;
    background-color: black;
}

</style>