<script>
import CardShoe from './CardShoe.vue';

export default {
    name: 'AppMainContainer',
    components: { CardShoe },
    data() {
        return {
            shoes: [
                { src: 'ad.jpg', name: 'Adidas Gazelle Indoor', price: '125 $' },
                { src: 'j11g.jpg', name: 'Jordan 11 Retro', price: '180$' },
                { src: 'ugg.jpg', name: 'UGG Tasman Slipper', price: '150$' },
                { src: 'mac.jpg', name: 'Nike Mac Attack', price: '240$' },
                { src: 'yz.jpg', name: 'Adidas Yeezy Slide', price: '80$' },
                { src: 'kb.jpg', name: 'Nike Kobe 6 Protro', price: '230$' },
            ]
        }
    }

}

</script>
<template>
    <section>
        <h2>Scarpe più Vendute</h2>
        <div class="container">
            <div class="box">
                <CardShoe class="product" v-for="shoe in shoes" :img="shoe.src" :title="shoe.name" :price="shoe.price"/>

            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/mixin.scss' as *;



section {
    @include bgImg('/nikes.jpg');

    padding: 3.75rem;
}

h2 {
    text-align: start;
    width: auto;
    text-shadow: 1px 1px 2px red;
    text-decoration: solid;
}

.box {
    display: flex;
    flex-wrap: nowrap;



    .product {
        flex-basis: calc(100% / 6);
        border: 1px solid black;
        background-color: white;

     
    }
 
}
</style>