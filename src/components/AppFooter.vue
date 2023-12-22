<script>
import AppFooterTrend from './AppFooterTrend.vue';
import AppFooterSettings from './AppFooterSettings.vue'
   export default{
name:'AppFooter',
components:{
   AppFooterTrend,
   AppFooterSettings,
}
   } 
</script>
<template>
    
<footer>
   <AppFooterTrend></AppFooterTrend>
   <AppFooterSettings></AppFooterSettings>
</footer>
</template>
<style lang="scss" scoped>
footer{
   background-color: green;
}
</style>
