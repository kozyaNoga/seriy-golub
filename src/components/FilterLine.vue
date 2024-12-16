<template>
    <div class="line">
        <p>Репродукции</p>
        <div>
            <button>Франция</button>
            <button>Германия</button>
            <button>Англия</button>
        </div>
    </div>
</template>

<script>
    export default{
        name: "FilterLine",
    }
</script>

<style>
    @media screen and (max-width: 2440px) {
        .line {
            flex-direction: row;
        }
        .line p {
            margin: 0% 0% 0% 0%;
        }
        .line div {
            justify-content: end;
        }
        .line button {
            font: lighter 12pt Verdana, sans-serif;
            padding: 0% 2% 0% 2%;
            margin: 0% 1.3% 0% 1.3%;
        }
    }

    @media screen and (max-width: 998px) {
        .line {
            flex-direction: row;
        }
        .line p {
            margin: 0% 0% 0% 0%;
        }
        .line div {
            justify-content: end;
        }
        .line button {
            font: lighter 14pt Verdana, sans-serif;
            padding: 2% 3% 2% 3%;
            margin: 0% 5% 0% 5%;
        }
    }

    @media screen and (max-width: 768px) {
        .line {
            flex-direction: column;
        }
        .line p {
            text-align: left;
            margin: 0% 0% 18pt 0%;
        }
        .line div {
            justify-content: flex-start;
        }
        .line button {
            font: lighter 14pt Verdana, sans-serif;
            padding: 2% 3% 2% 3%;
            margin: 0% 5% 0% 0%;
        }
    }

    @media screen and (max-width: 510px) {
    
    }
    .line {
        display:flex;
        flex-grow: 1;
        margin: 5pt 0% 15pt 0%;
    }

    .line p {
        
        font: lighter 20pt Verdana, sans-serif;
    }

    .line div {
        flex-grow: 2;
        display: flex;
    }
    
    .line button {
        border: 0px solid black;
        border-radius: 20px;
        background-color: #d4e8d9;
        
    }

    .line button:focus {
        background-color:#376b44;
        color: #f4f6f5;
        } 
</style>