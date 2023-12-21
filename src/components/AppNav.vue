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
            <li v-for="menu in menuList"><a :href="menu.link" :target="menu.target">{{menu.name}}</a></li>
         
            
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

nav {
    ul {
        margin: 0;
        list-style: none;
        display: flex;
    }

    a {
        display: inline-block;
        padding: 10px;
        background-color: $primary-color;

        &:hover {
            background-color: darken($primary-color, 10%);
        }
    }
}
</style>