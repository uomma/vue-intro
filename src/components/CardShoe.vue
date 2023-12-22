<script>
export default {
    name: 'CardShoe',
    props: {
        img: String,
        title: String,
        price: String,

    }
}
</script>
<template>
    <div class="card">
        <div><img :src="img"></div>
        <h5>{{title}}</h5>
        <h3>{{ price }}</h3>
    </div>
</template>
<style lang="scss" scoped>

img {
  padding-inline: 10px;
  max-width: 100%;
  height: 140px;
}
</style>