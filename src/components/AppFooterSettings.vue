<script>
export default {
    name: 'AppFooterSettings',
    data() {
        return {}
    }
}
</script>
<template>
    <footer>
        <button>
            <div class="regione">regione</div>
            <div> | </div>
            <div class="lingua">lingua</div>
            <div> | </div>
            <div class="valuta">valuta</div>
        </button>

        <div class="socials">
            <img src="/fb-lg.png" alt="fb">
            <img src="/ig-lg.png" alt="ig">
            <img src="/x-lg.png" alt="x">
            <img src="/yt-lg.png" alt="yt">
        </div>
        <div class="helpers">
            <div class="first">
                <a href="#">Guida</a><a href="#">Come Funziona</a><a href="#">Privacy</a><a href="#">Termini</a><a
                    href="#">Lavora Con Noi</a><a href="#">Contatti</a>
            </div>
            <div class="second">
                <a href="#">Suggerimenti prodotto</a><a href="#">Ufficio stampa</a><a href="#">ACCESSIBILITÀ</a>
            </div>
            <div class="third">
                <a href="">Diritti del Consumatore</a><a href="">Le tue preferenze per la Privacy</a>
            </div>
            <div class="fourth">©2023 StockY. Tutti i diritti riservati.</div>
        </div>
    </footer>
</template>
<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
@use 'sass:color';

footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-inline: 100px;
}



button {
    display: flex;
    padding: 5px;
    background-color: color.scale(black, $lightness: 10%);
    color: white;

    div {
        padding: 5px;
    }
}

.socials {
    width: 150px;
    height: 30px;
    display: flex;
    background-color: white;
    padding-inline: 10px;
}

.helpers {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    padding: 3px;

  
    a {
        text-decoration: none;
        padding-inline: 3px;
        color: black;
    }

}
</style>