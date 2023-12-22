<script>
export default {
    name: 'AppMainMenu',
    data() {
        return {
            categoryList: [

                {
                    name: 'Sneaker',
                    link: '#',
                    target: '_self',
                    isActive: false,

                }, {
                    name: 'Scarpe',
                    link: '#',
                    target: '_self',
                    isActive: false,
                }, {
                    name: 'Abbigliamento',
                    link: '#',
                    target: '_self',
                    isActive: false,
                }, {
                    name: 'Elettronica',
                    link: '#',
                    target: '_self',
                    isActive: false,
                }, {
                    name: 'Figurine',
                    link: '#',
                    target: '_self',
                    isActive: false,
                }, {
                    name: 'Collectibles',
                    link: '#',
                    target: '_self',
                    isActive: false,
                }, {
                    name: 'Accessori',
                    link: '#',
                    target: '_self',
                    isActive: false,
                }, {
                    name: 'Trending Deals',
                    link: '#',
                    target: '_self',
                    isActive: false,
                },
            ],
        }
    },
    methods: {
        changeMenu(index) {

            this.categoryList.forEach((element, i) => {
           
                if (index === i) {
                    element.isActive = true;
                } else {
                    element.isActive = false;
                }
            })
        },

     

    }

}
</script>
<template>
    <ul>
        <li v-for="(category, index) in categoryList">
            <a :class="{ active : category.isActive }" :href="category.link" :target="category.target"  @click.prevent="changeMenu(index)" >{{ category.name }}</a></li>
    </ul>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
@use 'sass:color';

ul {
    background-color: $secondary-color;
    margin: 0;
    list-style: none;
    display: flex;
    align-items: center;
    justify-content: center;

    li {
        padding-inline: 10px;
    }
}

a {
    display: inline-block;
    padding: 10px;
    color: #333;
    font-size: larger;
    text-decoration: none;

    &.active {
        background-color:  darken($secondary-color, 40%);

    }

    &:hover {
        background-color: darken($secondary-color, 20%);
        text-decoration: underline;
    }
}
</style>