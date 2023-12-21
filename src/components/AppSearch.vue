<script>
export default {
    name: 'AppSerach'
}

</script>
<template>
    <div class="search">
        <div class="ricerca">
            <button>
                <font-awesome-icon icon="fa-solid fa-magnifying-glass" class="icona" />

            </button>

            <input type="text" placeholder="cerca i tuoi articoli">
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

.ricerca {
    display: flex;
    align-items: center;

}

input {
    width: 750px;
    height: 37px;
    font-size: medium;
    background-color: $secondary-color ;

}

.icona {
    padding: 10px 10px 10px 10px;
    background-color: $secondary-color ;


}
</style>