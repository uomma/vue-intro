<script>
export default {
    name: 'AppFooterTrend',
    data() {
        return {
            trendList: [
                {
                    title: 'Air Jordan',
                    models: [
                        { name: 'Air Jordan 1' }, { name: 'Air Jordan 4' }, { name: 'Air Jordan 5' }, { name: 'Air Jordan 3' }, { name: 'Air Jordan 11' }, { name: 'Air Jordan 6' },
                    ]
                },
                {
                    title: 'Adidas',
                    models:[
                        {name:'Adidas Campus'}, {name:'Yeezy'}, {name:'Adidas Samba'}, {name:'Yeezy Slide'}, {name:'Adidas Gazelle'}, {name:'Adidas Forum'},
                    ]
                }
            ]
        }

    }
}
</script>

<template>  
    <ul v-for="trend in trendList">{{ trend.title }}
        <li v-for="model in trendList.models">{{ model.name }}</li>
    </ul>
</template>
<style lang="scss" scoped>


</style>