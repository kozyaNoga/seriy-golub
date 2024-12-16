<template>
    <div class="Big">
        <div class="pict"><img class="golub" src="../assets/bird.png"></div>
        <div class="text">
            <p class="Heading">Реплики картин<br>от Ink. House</p>
            <p class="Descriptions">Высокое качество отрисовки на плотной бумаге или льняном холсте. Редкие произведения, доступные цены.</p>
            <a class="prod" href="">Продукция</a>
        </div>
    </div>
</template>

<script>
export default{
    name: "BigItem",
}
</script>

<style>

    @media screen and (max-width: 2000px) {
        .golub {
            width: 100%;;
        }
        .text {
            padding: 10% 0% 10% 0%;
        }
        .Heading {
            font: lighter 24pt Verdana, sans-serif;
        }
        .Descriptions {
            padding: 0% 0% 0% 0%;
            font: lighter 9.5pt Verdana, sans-serif;
        }
        .prod {
            margin: 10% 0% 0% 0%;
        }
    }

    @media screen and (max-width: 998px) {
        .golub {
            width: 100%;;
        }
        .text {
            width: 50%;
            padding: 20pt 0% 0% 0%;
        }
        .pict {
            width: 50%;
        }
        .Heading {
            font: lighter 32pt Verdana, sans-serif;
        }
        .Descriptions {
            padding: 0% 0% 0% 0%;
            font: lighter 14pt Verdana, sans-serif;
        }
        .prod {
            margin: 10% 0% 0% 0%;
        }
    }

    @media screen and (max-width: 768px) {
        .golub {
            width: 100%;;
        }
        .pict {
            width: 50%;
            padding: 10% 0% 10% 0%;
        }
        .text {
            width: 50%;
            padding: 10% 0% 10% 0%;
        }
        .Heading {
            font: lighter 25pt Verdana, sans-serif;
        }
        .Descriptions {
            padding: 0% 0% 0% 0%;
            font: lighter 12pt Verdana, sans-serif;
        }
        .prod {
            margin: 5% 0% 0% 0%;
        }
    }

    @media screen and (max-width: 510px) {
        .golub {
            visibility: hidden;
        }
        .pict {
            width: 0%;
        }
        .text {
            width: 100%;
            padding: 20% 2% 0% 2%;
        }
        .Descriptions {
            font: lighter 14pt Verdana, sans-serif;
            padding: 0% 0% 8% 0%;
        }
        .prod {
            left: 0%;
            border: #80a78a 2px solid;
            padding: 3% 0% 3% 0%;
            width: 130pt;
            font-size: 17pt;
        }
    }
    .Big {
        display: flex;
    }
    img {

    }
    .Heading {
        padding: 0% 0% 0% 0%;
        margin: 0% 0% 0% 0%;
        text-align: left;
    }
    .Descriptions {
        
        margin: 5% 0% 0% 0%;
        text-align: left;
        line-height: 150%;
        color: #86928b;
    }
    .text {
        display: flex;
        flex-direction: column;
    }
    .prod {
        left: 0%;
        border: #80a78a 2px solid;
        padding: 3% 0% 3% 0%;
        width: 130pt;
    }
    .prod:link, .prod:visited {
        text-decoration: none;
        color: #80a78a;
    }

    .prod:active, .prod:hover {
        text-decoration: none;
        color: #80a78a;
    }
</style>