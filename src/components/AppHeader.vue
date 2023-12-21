<script>
import AppLogo from './AppLogo.vue';
import AppNav from './AppNav.vue';
export default {
    name: 'AppHeader',
    components: {
        AppLogo,
        AppNav
    }
} 
</script>
<template>
    <header>
        <div>
            <AppLogo></AppLogo>
        </div>
        <nav><AppNav></AppNav></nav>
    </header>
</template>