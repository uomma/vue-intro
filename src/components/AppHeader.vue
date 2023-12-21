<script>
import AppLogo from './AppLogo.vue';
import AppNav from './AppNav.vue';
import AppSearch from './AppSearch.vue';
export default {
    name: 'AppHeader',
    components: {
        AppLogo,
        AppNav,
        AppSearch
    }
} 
</script>
<template>
    <header>
        <div>
            <AppLogo></AppLogo>
            
        </div>
        <div><AppSearch></AppSearch></div>
        <nav><AppNav></AppNav></nav>
        
    </header>
</template>
<style lang="scss" scoped>
header{
    display: flex;
    justify-content: space-between;
    align-items: center;

  

}

</style>