<script>
export default {
    name: 'AppMainMenu',
    data() {
        return {
            categoryList: [

                {
                    name: 'Sneaker',
                    link: '#',
                    target: '_self'
                }, {
                    name: 'Scarpe',
                    link: '#',
                    target: '_self'
                }, {
                    name: 'Abbigliamento',
                    link: '#',
                    target: '_self'
                }, {
                    name: 'Elettronica',
                    link: '#',
                    target: '_self'
                }, {
                    name: 'Figurine',
                    link: '#',
                    target: '_self'
                }, {
                    name: 'Collectibles',
                    link: '#',
                    target: '_self'
                }, {
                    name: 'Accessori',
                    link: '#',
                    target: '_self'
                }, {
                    name: 'Trending Deals',
                    link: '#',
                    target: '_self'
                },
            ],
        }
    }

}
</script>
<template>
    <ul>
        <li v-for="category in categoryList"><a :href="category.link" :target="category.target">{{ category.name }}</a></li>
    </ul>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
@use 'sass:color';

ul {
    margin: 0;
    list-style: none;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: $secondary-color;

    li {
        padding-inline: 10px;
    }
}

a {
    display: inline-block;
    padding: 10px;
    background-color: $secondary-color;
    color: #333;
    font-size: larger;


    &:hover {
        background-color: darken($secondary-color, 20%);
    }
}
</style>