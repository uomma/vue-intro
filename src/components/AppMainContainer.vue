<script>
export default {
    name: 'AppMainContainer',

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
                <div class="card" v-for="shoe in shoes">
                    <div class="img"><img :src="shoe.src" alt=""></div>
                    <h6>{{ shoe.name }}</h6>
                    <h3>{{ shoe.price }}</h3>

                </div>

            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/mixin.scss' as *;

section {
    @include bgImg('/nikes.jpg');

    background-color: red;
    padding: 3.75rem;
}

h2 {
    text-align: center;
}

.box {
    display: flex;
    flex-wrap: nowrap;
    


    .card {
        flex-basis: calc(100% / 6);
        border: 1px solid black;
        background-color: yellow;

        img {
            padding-inline: 10px;
            width: 200px;
            height: 140px ;
        }
    }
}
</style>