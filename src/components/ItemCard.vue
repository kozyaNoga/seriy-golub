<template>
    <a id="ref" href="">
        <div id="card">
            <div class="chue"><img :src="require(`@/assets/france/${url}`)" /></div>
            <div class="text_card">
                <p class=name_artist>{{ name_artist }}</p>
                <p class=name_picture>{{ name_picture }}</p>
                <p class="material">{{ material }}</p>
                <p class="price">{{ price }}</p>
            </div>
            <button>В корзину</button>
        </div>
    </a>
    
</template>

<script>
    export default {
        name: "ItemCard",
        props: {
            name_artist: String,
            name_picture: String,
            material: String, 
            price: String,
            url: String
        }
    }
</script>

<style>
    #ref:link, #ref:visited {
        text-decoration: none;
        padding: 0% 0% 0% 0%;
        margin: 0% 0% 0% 0%;
        color: 
    }

    #ref:active, #ref:hover {
        text-decoration: none;
        padding: 0% 0% 0% 0%;
        margin: 0% 0% 0% 0%;
    }

    #card {
        background-color: #e1ede6;
        padding: 0% 0% 0% 0%;
        margin: 1% 1% 1% 1%;
        width: 100%;
    }

    .chue img {
        width: 88%;
        margin: 6.5% 0% 0% 0%;
    }
     
    #card button {
        font: lighter 14pt Verdana, sans-serif;
        width: 88%;
        padding: 6% 0% 6% 0%;
        margin: 6% 0% 6% 0%;
        border: 1px solid #598d66;
        border-radius: 0px;
        background-color: #e1ede6;
        color: #598d66;
    }

    .text_card {
        width: 100%;
        margin: 0% 0% 0% 7%;
    }

    .text_card p {
        text-align: left;
    }

    .name_artist {
        font: lighter 10pt Verdana, sans-serif;
        color: #86928b;
    }

    .name_picture{
        margin: 0% 0% 0% 0%;
        font: lighter 17pt Verdana, sans-serif;
        color: #2c2d35;
    }

    .material {
        margin: 2% 0% 0% 0%;
        font: lighter 10pt Verdana, sans-serif;
        color: #2c2d35;
    }

    .price {
        margin: 10% 0% 0% 0%;
        font: lighter 13pt Verdana, sans-serif;
        color: #598d66;
    }
</style>