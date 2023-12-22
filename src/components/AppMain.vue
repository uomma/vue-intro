<script>
import AppMainMenu from './AppMainMenu.vue';
import AppMainContainer from './AppMainContainer.vue';
export default {
    name: 'AppMain',
    components: {
        AppMainMenu,
        AppMainContainer
    }

} 
</script>
<template><main>
    <AppMainMenu></AppMainMenu>
    <AppMainContainer></AppMainContainer>

</main>
</template>
<style lang="scss" scoped>


</style>