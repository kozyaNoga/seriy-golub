<template>
        <div class="grad">
            
            <div class="promo">
                <div class="text_promo">
                    <p id="title">Новая коллекция французских авторов</p>
                    <p>Сложно сказать, почему акционеры крупнейших компаний призывают нас к новым свершениям, которые, в свою очередь, должны быть заблокированы в рамках своих собственных рациональных ограничений.</p>
                    <p>Принимая во внимание показатели успешности, граница обучения кадров предопределяет высокую востребованность направлений прогрессивного развития.</p>
                    <button id="promo_button">Ознакомиться</button>
                </div>
            </div>
        </div> 
        <div>
            <div class="unpromo">
                <div class="unpromo_picture">
                    <img class="unpromo_picture_rama" src="../assets/rama.png" alt="">
                    <img class="unpromo_picture_hand" src="../assets/Hand.png" alt="">
                </div>
                <div class="unpromo_text">
                    <p class="unpromo_text_title">Наша команда</p>
                    <p class="unpromo_text_text">Значимость этих проблем настолько очевидна, что базовый вектор развития позволяет оценить значение экспериментов, поражающих по своей масштабности и грандиозности. Мы вынуждены отталкиваться от того, что консультация c широким активом.</p>
                    <img class="ellipse" src="../assets/ellipse.png" alt="">
                </div>
            </div>
        </div>
</template>

<script>
    export default {
        name: "PromoItem",
    }
</script>

<style>
    @media screen and (max-width: 2440px) {
        .promo .text_promo {
            padding: 1% 0% 0% 13%;
            width: 50%;
        }

        #promo_button {
            padding: 3% 0% 3% 0%;
            margin: 8% 0% 0% 0%;
            width: 40%;
        }

        .unpromo {
            margin: 4% 13% 10% 13%;
            display: flex;
        }  
        
        .unpromo_picture {
            max-width: 50%;
            height: 200pt;
        }
        .unpromo_text {
            max-width: 100%;
            margin: 0% 0% 0% 0%;
            padding: 5% 0% 0% 40%;
            text-align: left;
        }

        .unpromo_picture_rama {
            max-width: 28%;
            padding-top: 5%;
        }

        .unpromo_picture_hand {
            max-width: 17%;
            padding-left: 3%;
        }

        .ellipse {
            max-width: 55%;
        }

    }

    @media screen and (max-width: 998px) {
        .promo .text_promo {
            padding: 1% 0% 0% 7%;
            width: 90%;
        }

        #promo_button {
            padding: 2% 0% 2% 0%;
            margin: 5% 0% 0% 0%;
            width: 25%;
        }

        .unpromo {
            margin: 4% 7% 10% 7%;
            display: block;
        }

        .unpromo_picture {
            max-width: 50%;
        }

        .unpromo_text {
            max-width: 100%;
            margin: 30% 0% 0% 0%;
            padding: 5% 0% 0% 0%;
            text-align: left;
        }
        
        .unpromo_picture_rama {
            max-width: 58%;
            left: 7%;
            padding-top: 10%;
        }

        .unpromo_picture_hand {
            max-width: 35%;
            left: 7%;
            padding-left: 6%;
        }

        .ellipse {
            max-width: 55%;
        }

    }

    @media screen and (max-width: 768px) {
        #promo_button {
            padding: 3% 0% 3% 0%;
            margin: 5% 0% 0% 0%;
            width: 34%;
        }

        .unpromo_text {
            max-width: 100%;
            margin: 20% 0% 0% 0%;
            padding: 5% 0% 0% 0%;
            text-align: left;
        }

        .ellipse {
            max-width: 55%;
        }

    }

    @media screen and (max-width: 510px) {
        #promo_button {
            padding: 3% 0% 3% 0%;
            margin: 5% 0% 0% 0%;
            width: 100%;
        }

        .unpromo_text {
            max-width: 100%;
            margin: 28% 0% 0% 0%;
            padding: 5% 0% 0% 0%;
            text-align: left;
        }

        .unpromo_picture_rama {
            max-width: 86%;
            left: 7%;
            padding-top: 12%;
        }

        .unpromo_picture_hand {
            max-width: 50%;
            left: 10%;
            padding-left: 6%;
        }

        .ellipse {
            max-width: 100%;
        }

    }

    .grad {
        width: 100%;
        height: 100%;
        display: inline-block;
        position: relative;    
    }

    .promo {
        width: 100%;
        height: 350pt;
        background-image: url("../assets/promo.jpg");
        background-size: cover;
    }

    .promo :not(.text_promo) {
        
        color: white;
        z-index: 1;
        position: relative;
        top: 0%;
    }

    .promo .text_promo {
        text-align: left;
    }

    .grad:after {
        content: "";
        display: block;    
        width: 100%;
        height: 100%;    
        position: absolute;
        top: 0;      
        left: 0;   
        background: transparent;
        background-image: linear-gradient(to right, #03090e, transparent);
        background-size: cover;
        opacity: 0.8;
    }
    
    #title {
        font: lighter 16pt Verdana, sans-serif;
    }

    #promo_button {
        border: 0px solid black;
        color: #2c2d35;
        background-color: #eedb6d;
        font: lighter 14pt Verdana, sans-serif;
    }

    .unpromo_picture_rama {
        position: absolute;
    }

    .unpromo_picture_hand {
        position: absolute;
    }

    .unpromo_text_title {
        font: lighter 17pt Verdana, sans-serif;
    }

    .unpromo_text_text {
        font: lighter 10pt Verdana, sans-serif;
    }


</style>