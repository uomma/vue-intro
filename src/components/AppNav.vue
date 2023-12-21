<script>
export default {
    name: 'AppNav',
    data() {
        return {
            menuList: [
                {
                    name: 'Esplora',
                    link: '#',
                    target: '_self'
                },
                {
                    name: 'Notizie',
                    link: '#',
                    target: '_self'
                }, {
                    name: 'Info',
                    link: '#',
                    target: '_self'
                }, {
                    name: 'Guida',
                    link: '#',
                    target: '_self'
                }, {
                    name: 'Vendi',
                    link: '#',
                    target: '_self'
                },

            ]
        }
    }
}
</script>
<template>
    <nav>
        <ul>
            <li v-for="menu in menuList"><a :href="menu.link" :target="menu.target">{{ menu.name }}</a></li>
            <a href=""><font-awesome-icon icon="fa-regular fa-heart" /></a>
            <a href=""><font-awesome-icon icon="fa-regular fa-bell" /></a>
            <a href=""><font-awesome-icon icon="fa-regular fa-user" /></a>

        </ul>

    </nav>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
@use 'sass:color' ;

nav {
    
   
    ul {
        margin: 0;
        list-style: none;
        display: flex;
        align-items: center;
        justify-content: flex-end;       
        
        li{
            padding-inline: 10px ;
            background-color: $primary-color;
        }
    }

    

    a {
        display: inline-block;
        padding: 10px;
        background-color: $primary-color;
        color: white;
       

        &:hover {
            background-color: color.scale($primary-color, $lightness: 10%);
        }
    }
}
</style>